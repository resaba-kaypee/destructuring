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
