# destructuring
//#destructuring
const voxel = {
x: 11,
y: 22,
z: 33
}
const {x ,y ,z } = voxel;
console.log(x) //return 11

//#assign values to another variable
const { x : a, y : b, z : c } = voxel
console.log(a) //return 11



//#assign variables from object
const AVG_TEMPERATURE = {
today: 77.5,
tomorrow; 79
}

function getTemOfTomorrow(avgTemp){
const { tomorrow : tempOfTomorrow } = avgTemp;
return tempOfTomorrow;

console.log(getTemOfTomorrow(AVG_TEMPERATURE))

//#assign variables from nested objects

const LOCAL_FORECAST = {
today : { min: 5, max: 10 },
tomorrow : { min 15, max: 20}
};

function getMaxOfTom(forecast) {
const {tomorrow : { max : maxTempOfTom }} = forecast;
return maxTempOfTom;

console.log(getMaxOfTom(LOCAL_FORECAST));

//#assign variables from array

const [a, b] = [1, 2, 3, 4, 5]
console.log(a, b) // [1, 2]

const [a, b,,, c] = [1, 2, 3, 4, 5, 6]
console.log(a, b, c)// [1, 2, 5]

//#using rest operator to reassign the array elements

const source = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
function removeTheFirstTwo(list) {
const [a, b, ...arr] = list;
return arr;
}
const arr = removeTheFirstTwo(source);
console.log(arr);
console.log(source)


