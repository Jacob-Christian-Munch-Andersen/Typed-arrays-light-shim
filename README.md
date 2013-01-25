Typed-arrays-light-shim
=======================

Some of the functionality of typed arrays implemented as an overlay on arrays.

The intention of this project is to provide an approximate subset of JavaScript typed arrays that let developers gain some of the advantages of typed arrays, while maintaining support for browsers that do not support typed arrays, and also maintaining reasonable performance in these browsers.

It is released under a BSD licence.

Notable features not present:
=============================
No datatype conversion, all array types implement 64 bit floats.<br>
subarray does not provide a view for an arraybuffer, rather it makes a new array.<br>
No checks for illegal operations, where the specification would throw an error this code will most likely continue.<br>
No ArrayBuffer objects, typed arrays are implemented as independent objects.<br>
Lots of little things like toString that shouldn't matter for normal use.

Notable features:
=================
Works in IE 7, 8 and 9.<br>
Good performance.
