cache.js
========

cache.js is a javascript prototype function that caches the return of a 
function + args.

!!! It doesn't do anything else than storing the return of a function 
in a hash

Example :
var test = function (x) {
 return x;
}

test.cache(1); // execute test(1) function a first time
test.cache(1); // return the content of cache
test.cache(2); // execute test(2) another time because arguments 
               // have changed