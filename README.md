# High-order-functions

function iAmCallbackFunction() {
 console.log("callback has been invoked");
}
function iAmJustFunction(callbackFn) {
 // do some stuff ...
 // invoke the callback function.
 callbackFn();
}
// invoke your higher-order function with a callback function.
iAmJustFunction(iAmCallbackFunction);
A higher-order function is also a function that returns another function as its result.
function iAmJustFunction() {
 // do some stuff ...
 // return a function.
 return function iAmReturnedFunction() {
 console.log("returned function has been invoked");
 }
}
// invoke your higher-order function and its returned function.
iAmJustFunction()();
