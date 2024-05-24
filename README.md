<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Assert

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Assertion utilities.

<section class="installation">

## Installation

```bash
npm install @taktikangea/blanditiis-nemo
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var assert = require( '@taktikangea/blanditiis-nemo' );
```

#### assert

Namespace providing utilities for data type testing and feature detection.

```javascript
var o = assert;
// returns {...}
```

To validate the built-in JavaScript data types, the namespace includes the following assertion utilities:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArray( value )`][@taktikangea/blanditiis-nemo/is-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array.</span>
-   <span class="signature">[`isBoolean( value )`][@taktikangea/blanditiis-nemo/is-boolean]</span><span class="delimiter">: </span><span class="description">test if a value is a boolean.</span>
-   <span class="signature">[`isDateObject( value )`][@taktikangea/blanditiis-nemo/is-date-object]</span><span class="delimiter">: </span><span class="description">test if a value is a Date object.</span>
-   <span class="signature">[`isFunction( value )`][@taktikangea/blanditiis-nemo/is-function]</span><span class="delimiter">: </span><span class="description">test if a value is a function.</span>
-   <span class="signature">[`isnan( value )`][@taktikangea/blanditiis-nemo/is-nan]</span><span class="delimiter">: </span><span class="description">test if a value is NaN.</span>
-   <span class="signature">[`isNull( value )`][@taktikangea/blanditiis-nemo/is-null]</span><span class="delimiter">: </span><span class="description">test if a value is null.</span>
-   <span class="signature">[`isNumber( value )`][@taktikangea/blanditiis-nemo/is-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number.</span>
-   <span class="signature">[`isObject( value )`][@taktikangea/blanditiis-nemo/is-object]</span><span class="delimiter">: </span><span class="description">test if a value is an object.</span>
-   <span class="signature">[`isRegExp( value )`][@taktikangea/blanditiis-nemo/is-regexp]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression.</span>
-   <span class="signature">[`isString( value )`][@taktikangea/blanditiis-nemo/is-string]</span><span class="delimiter">: </span><span class="description">test if a value is a string.</span>
-   <span class="signature">[`isSymbol( value )`][@taktikangea/blanditiis-nemo/is-symbol]</span><span class="delimiter">: </span><span class="description">test if a value is a symbol.</span>
-   <span class="signature">[`isUndefined( value )`][@taktikangea/blanditiis-nemo/is-undefined]</span><span class="delimiter">: </span><span class="description">test if a value is undefined.</span>

</div>

<!-- </toc> -->

For primitive types having corresponding object wrappers, assertion utilities provide `isObject` and `isPrimitive` methods to test for either objects or primitives, respectively.

<!-- eslint-disable no-new-wrappers -->

```javascript
var Boolean = require( '@stdlib/boolean/ctor' );
var isBoolean = require( '@taktikangea/blanditiis-nemo/is-boolean' );

var bool = isBoolean.isObject( new Boolean( false ) );
// returns true

bool = isBoolean.isObject( false );
// returns false

bool = isBoolean.isPrimitive( false );
// returns true
```

Many of the assertion utilities have corresponding packages that test whether array elements are of the given data type:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|nan|number|object|regexp|symbol|null|undefined)-array" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArrayArray( value )`][@taktikangea/blanditiis-nemo/is-array-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of arrays.</span>
-   <span class="signature">[`isBooleanArray( value )`][@taktikangea/blanditiis-nemo/is-boolean-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of booleans.</span>
-   <span class="signature">[`isDateObjectArray( value )`][@taktikangea/blanditiis-nemo/is-date-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only Date objects.</span>
-   <span class="signature">[`isFunctionArray( value )`][@taktikangea/blanditiis-nemo/is-function-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only functions.</span>
-   <span class="signature">[`isNaNArray( value )`][@taktikangea/blanditiis-nemo/is-nan-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only NaN values.</span>
-   <span class="signature">[`isNullArray( value )`][@taktikangea/blanditiis-nemo/is-null-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only null values.</span>
-   <span class="signature">[`isNumberArray( value )`][@taktikangea/blanditiis-nemo/is-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of numbers.</span>
-   <span class="signature">[`isObjectArray( value )`][@taktikangea/blanditiis-nemo/is-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only objects.</span>
-   <span class="signature">[`isStringArray( value )`][@taktikangea/blanditiis-nemo/is-string-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of strings.</span>
-   <span class="signature">[`isSymbolArray( value )`][@taktikangea/blanditiis-nemo/is-symbol-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only symbols.</span>

</div>

<!-- </toc> -->

Where applicable, similar to the assertion utilities for built-in data types, array assertion utilities provides methods for testing for an array of primitives or objects.

<!-- eslint-disable no-new-wrappers -->

```javascript
var isStringArray = require( '@taktikangea/blanditiis-nemo/is-string-array' );

var bool = isStringArray( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.primitives( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.objects( [ 'hello', 'world' ] );
// returns false

bool = isStringArray.objects( [ new String( 'hello' ), new String( 'world' ) ] );
// returns true
```

The namespace also contains utilities to test for numbers within a certain range or for numbers satisfying a particular "type":

<!-- <toc pattern="is-*+(number|integer)*" ignore="is-number-array" ignore="is-number" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCubeNumber( value )`][@taktikangea/blanditiis-nemo/is-cube-number]</span><span class="delimiter">: </span><span class="description">test if a value is a cube number.</span>
-   <span class="signature">[`isIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only integers.</span>
-   <span class="signature">[`isInteger( value )`][@taktikangea/blanditiis-nemo/is-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having an integer value.</span>
-   <span class="signature">[`isNegativeIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-negative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative integers.</span>
-   <span class="signature">[`isNegativeInteger( value )`][@taktikangea/blanditiis-nemo/is-negative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative integer value.</span>
-   <span class="signature">[`isNegativeNumberArray( value )`][@taktikangea/blanditiis-nemo/is-negative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative numbers.</span>
-   <span class="signature">[`isNegativeNumber( value )`][@taktikangea/blanditiis-nemo/is-negative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative value.</span>
-   <span class="signature">[`isNonNegativeIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-nonnegative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative integers.</span>
-   <span class="signature">[`isNonNegativeInteger( value )`][@taktikangea/blanditiis-nemo/is-nonnegative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative integer value.</span>
-   <span class="signature">[`isNonNegativeNumberArray( value )`][@taktikangea/blanditiis-nemo/is-nonnegative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative numbers.</span>
-   <span class="signature">[`isNonNegativeNumber( value )`][@taktikangea/blanditiis-nemo/is-nonnegative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative value.</span>
-   <span class="signature">[`isNonPositiveIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-nonpositive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive integers.</span>
-   <span class="signature">[`isNonPositiveInteger( value )`][@taktikangea/blanditiis-nemo/is-nonpositive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive integer value.</span>
-   <span class="signature">[`isNonPositiveNumberArray( value )`][@taktikangea/blanditiis-nemo/is-nonpositive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive numbers.</span>
-   <span class="signature">[`isNonPositiveNumber( value )`][@taktikangea/blanditiis-nemo/is-nonpositive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive value.</span>
-   <span class="signature">[`isPositiveIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-positive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive integers.</span>
-   <span class="signature">[`isPositiveInteger( value )`][@taktikangea/blanditiis-nemo/is-positive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive integer value.</span>
-   <span class="signature">[`isPositiveNumberArray( value )`][@taktikangea/blanditiis-nemo/is-positive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive numbers.</span>
-   <span class="signature">[`isPositiveNumber( value )`][@taktikangea/blanditiis-nemo/is-positive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive value.</span>
-   <span class="signature">[`isSafeIntegerArray( value )`][@taktikangea/blanditiis-nemo/is-safe-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only safe integers.</span>
-   <span class="signature">[`isSafeInteger( value )`][@taktikangea/blanditiis-nemo/is-safe-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a safe integer value.</span>
-   <span class="signature">[`isSquareNumber( value )`][@taktikangea/blanditiis-nemo/is-square-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square number.</span>
-   <span class="signature">[`isSquareTriangularNumber( value )`][@taktikangea/blanditiis-nemo/is-square-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square triangular number.</span>
-   <span class="signature">[`isTriangularNumber( value )`][@taktikangea/blanditiis-nemo/is-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a triangular number.</span>

</div>

<!-- </toc> -->

The namespace provides utilities for validating typed arrays:

<!-- <toc pattern="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array"> -->

<div class="namespace-toc">

-   <span class="signature">[`isFloat32Array( value )`][@taktikangea/blanditiis-nemo/is-float32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float32Array.</span>
-   <span class="signature">[`isFloat64Array( value )`][@taktikangea/blanditiis-nemo/is-float64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float64Array.</span>
-   <span class="signature">[`isInt16Array( value )`][@taktikangea/blanditiis-nemo/is-int16array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int16Array.</span>
-   <span class="signature">[`isInt32Array( value )`][@taktikangea/blanditiis-nemo/is-int32array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int32Array.</span>
-   <span class="signature">[`isInt8Array( value )`][@taktikangea/blanditiis-nemo/is-int8array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int8Array.</span>
-   <span class="signature">[`isUint16Array( value )`][@taktikangea/blanditiis-nemo/is-uint16array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint16Array.</span>
-   <span class="signature">[`isUint32Array( value )`][@taktikangea/blanditiis-nemo/is-uint32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint32Array.</span>
-   <span class="signature">[`isUint8Array( value )`][@taktikangea/blanditiis-nemo/is-uint8array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8Array.</span>
-   <span class="signature">[`isUint8ClampedArray( value )`][@taktikangea/blanditiis-nemo/is-uint8clampedarray]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8ClampedArray.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating `ndarray`s (n-dimensional arrays).

<!-- <toc keywords="+ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCentrosymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a centrosymmetric matrix.</span>
-   <span class="signature">[`isComplex128MatrixLike( value )`][@taktikangea/blanditiis-nemo/is-complex128matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128ndarrayLike( value )`][@taktikangea/blanditiis-nemo/is-complex128ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128VectorLike( value )`][@taktikangea/blanditiis-nemo/is-complex128vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64MatrixLike( value )`][@taktikangea/blanditiis-nemo/is-complex64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64ndarrayLike( value )`][@taktikangea/blanditiis-nemo/is-complex64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64VectorLike( value )`][@taktikangea/blanditiis-nemo/is-complex64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isFloat32MatrixLike( value )`][@taktikangea/blanditiis-nemo/is-float32matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32ndarrayLike( value )`][@taktikangea/blanditiis-nemo/is-float32ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32VectorLike( value )`][@taktikangea/blanditiis-nemo/is-float32vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64MatrixLike( value )`][@taktikangea/blanditiis-nemo/is-float64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64ndarrayLike( value )`][@taktikangea/blanditiis-nemo/is-float64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64VectorLike( value )`][@taktikangea/blanditiis-nemo/is-float64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isMatrixLike( value )`][@taktikangea/blanditiis-nemo/is-matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is 2-dimensional ndarray-like object.</span>
-   <span class="signature">[`isndarrayLike( value )`][@taktikangea/blanditiis-nemo/is-ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is ndarray-like.</span>
-   <span class="signature">[`isNonSymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-nonsymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a non-symmetric matrix.</span>
-   <span class="signature">[`isPersymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a persymmetric matrix.</span>
-   <span class="signature">[`isSkewCentrosymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-skew-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-centrosymmetric matrix.</span>
-   <span class="signature">[`isSkewPersymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-skew-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-persymmetric matrix.</span>
-   <span class="signature">[`isSkewSymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-skew-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-symmetric matrix.</span>
-   <span class="signature">[`isSquareMatrix( value )`][@taktikangea/blanditiis-nemo/is-square-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object having equal dimensions.</span>
-   <span class="signature">[`isSymmetricMatrix( value )`][@taktikangea/blanditiis-nemo/is-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a symmetric matrix.</span>
-   <span class="signature">[`isVectorLike( value )`][@taktikangea/blanditiis-nemo/is-vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating complex numbers and arrays of complex numbers:

<!-- <toc pattern="is-complex*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isComplexLike( value )`][@taktikangea/blanditiis-nemo/is-complex-like]</span><span class="delimiter">: </span><span class="description">test if a value is a complex number-like object.</span>
-   <span class="signature">[`isComplexTypedArrayLike( value )`][@taktikangea/blanditiis-nemo/is-complex-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is complex-typed-array-like.</span>
-   <span class="signature">[`isComplexTypedArray( value )`][@taktikangea/blanditiis-nemo/is-complex-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a complex typed array.</span>
-   <span class="signature">[`isComplex( value )`][@taktikangea/blanditiis-nemo/is-complex]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit or 128-bit complex number.</span>
-   <span class="signature">[`isComplex128( value )`][@taktikangea/blanditiis-nemo/is-complex128]</span><span class="delimiter">: </span><span class="description">test if a value is a 128-bit complex number.</span>
-   <span class="signature">[`isComplex128Array( value )`][@taktikangea/blanditiis-nemo/is-complex128array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex128Array.</span>
-   <span class="signature">[`isComplex64( value )`][@taktikangea/blanditiis-nemo/is-complex64]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit complex number.</span>
-   <span class="signature">[`isComplex64Array( value )`][@taktikangea/blanditiis-nemo/is-complex64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex64Array.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating other special arrays or buffers:

<!-- <toc pattern="is-*array*" ignore="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array" ignore="is-*+(number|integer)*" ignore="is-+(array|boolean|date-object|function|string|nan|number|object|primitive|regexp|symbol|null|undefined)-array" ignore="is-array" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isAccessorArray( value )`][@taktikangea/blanditiis-nemo/is-accessor-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object supporting the accessor (get/set) protocol.</span>
-   <span class="signature">[`isArrayLength( value )`][@taktikangea/blanditiis-nemo/is-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid array length.</span>
-   <span class="signature">[`isArrayLikeObject( value )`][@taktikangea/blanditiis-nemo/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>
-   <span class="signature">[`isArrayLike( value )`][@taktikangea/blanditiis-nemo/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>
-   <span class="signature">[`isArrayBufferView( value )`][@taktikangea/blanditiis-nemo/is-arraybuffer-view]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer view.</span>
-   <span class="signature">[`isArrayBuffer( value )`][@taktikangea/blanditiis-nemo/is-arraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer.</span>
-   <span class="signature">[`isBetweenArray( value, a, b[, left, right] )`][@taktikangea/blanditiis-nemo/is-between-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object where every element is between two values.</span>
-   <span class="signature">[`isBigInt64Array( value )`][@taktikangea/blanditiis-nemo/is-bigint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt64Array.</span>
-   <span class="signature">[`isBigUint64Array( value )`][@taktikangea/blanditiis-nemo/is-biguint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigUint64Array.</span>
-   <span class="signature">[`isCircularArray( value )`][@taktikangea/blanditiis-nemo/is-circular-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array containing a circular reference.</span>
-   <span class="signature">[`isEmptyArrayLikeObject( value )`][@taktikangea/blanditiis-nemo/is-empty-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array-like object.</span>
-   <span class="signature">[`isEmptyArray( value )`][@taktikangea/blanditiis-nemo/is-empty-array]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array.</span>
-   <span class="signature">[`isFalsyArray( value )`][@taktikangea/blanditiis-nemo/is-falsy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only falsy values.</span>
-   <span class="signature">[`isFiniteArray( value )`][@taktikangea/blanditiis-nemo/is-finite-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only finite numbers.</span>
-   <span class="signature">[`isNumericArray( value )`][@taktikangea/blanditiis-nemo/is-numeric-array]</span><span class="delimiter">: </span><span class="description">test if a value is a numeric array.</span>
-   <span class="signature">[`isPlainObjectArray( value )`][@taktikangea/blanditiis-nemo/is-plain-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only plain objects.</span>
-   <span class="signature">[`isProbabilityArray( value )`][@taktikangea/blanditiis-nemo/is-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only probabilities.</span>
-   <span class="signature">[`isSameArray( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both generic arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex128Array( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-complex128array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex128Arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex64Array( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-complex64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex64Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat32Array( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-float32array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float32Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat64Array( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-float64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float64Arrays and have the same values.</span>
-   <span class="signature">[`isSharedArrayBuffer( value )`][@taktikangea/blanditiis-nemo/is-sharedarraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is a SharedArrayBuffer.</span>
-   <span class="signature">[`isTruthyArray( value )`][@taktikangea/blanditiis-nemo/is-truthy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only truthy values.</span>
-   <span class="signature">[`isTypedArrayLength( value )`][@taktikangea/blanditiis-nemo/is-typed-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid typed array length.</span>
-   <span class="signature">[`isTypedArrayLike( value )`][@taktikangea/blanditiis-nemo/is-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is typed-array-like.</span>
-   <span class="signature">[`isTypedArray( value )`][@taktikangea/blanditiis-nemo/is-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a typed array.</span>
-   <span class="signature">[`isUnityProbabilityArray( value )`][@taktikangea/blanditiis-nemo/is-unity-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of probabilities that sum to one.</span>

</div>

<!-- </toc> -->

To test for error objects, the namespace includes the following utilities:

<!-- <toc pattern="is-*error*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isError( value )`][@taktikangea/blanditiis-nemo/is-error]</span><span class="delimiter">: </span><span class="description">test if a value is an Error object.</span>
-   <span class="signature">[`isEvalError( value )`][@taktikangea/blanditiis-nemo/is-eval-error]</span><span class="delimiter">: </span><span class="description">test if a value is an EvalError object.</span>
-   <span class="signature">[`isRangeError( value )`][@taktikangea/blanditiis-nemo/is-range-error]</span><span class="delimiter">: </span><span class="description">test if a value is a RangeError object.</span>
-   <span class="signature">[`isReferenceError( value )`][@taktikangea/blanditiis-nemo/is-reference-error]</span><span class="delimiter">: </span><span class="description">test if a value is a ReferenceError object.</span>
-   <span class="signature">[`isSyntaxError( value )`][@taktikangea/blanditiis-nemo/is-syntax-error]</span><span class="delimiter">: </span><span class="description">test if a value is a SyntaxError object.</span>
-   <span class="signature">[`isTypeError( value )`][@taktikangea/blanditiis-nemo/is-type-error]</span><span class="delimiter">: </span><span class="description">test if a value is a TypeError object.</span>
-   <span class="signature">[`isURIError( value )`][@taktikangea/blanditiis-nemo/is-uri-error]</span><span class="delimiter">: </span><span class="description">test if a value is a URIError object.</span>

</div>

<!-- </toc> -->

The namespace exposes the following constants concerning the current running process:

<!-- <toc pattern="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|big-endian|node|web-worker|windows|docker|mobile|touch-device)" > -->

<div class="namespace-toc">

-   <span class="signature">[`IS_BIG_ENDIAN`][@taktikangea/blanditiis-nemo/is-big-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is big endian.</span>
-   <span class="signature">[`IS_BROWSER`][@taktikangea/blanditiis-nemo/is-browser]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web browser.</span>
-   <span class="signature">[`IS_DARWIN`][@taktikangea/blanditiis-nemo/is-darwin]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Darwin.</span>
-   <span class="signature">[`IS_DOCKER`][@taktikangea/blanditiis-nemo/is-docker]</span><span class="delimiter">: </span><span class="description">check if the process is running in a Docker container.</span>
-   <span class="signature">[`IS_ELECTRON_MAIN`][@taktikangea/blanditiis-nemo/is-electron-main]</span><span class="delimiter">: </span><span class="description">check if the runtime is the main Electron process.</span>
-   <span class="signature">[`IS_ELECTRON_RENDERER`][@taktikangea/blanditiis-nemo/is-electron-renderer]</span><span class="delimiter">: </span><span class="description">check if the runtime is the Electron renderer process.</span>
-   <span class="signature">[`IS_ELECTRON`][@taktikangea/blanditiis-nemo/is-electron]</span><span class="delimiter">: </span><span class="description">check if the runtime is Electron.</span>
-   <span class="signature">[`IS_LITTLE_ENDIAN`][@taktikangea/blanditiis-nemo/is-little-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is little endian.</span>
-   <span class="signature">[`IS_MOBILE`][@taktikangea/blanditiis-nemo/is-mobile]</span><span class="delimiter">: </span><span class="description">check if the current environment is a mobile device.</span>
-   <span class="signature">[`IS_NODE`][@taktikangea/blanditiis-nemo/is-node]</span><span class="delimiter">: </span><span class="description">check if the runtime is Node.js.</span>
-   <span class="signature">[`IS_TOUCH_DEVICE`][@taktikangea/blanditiis-nemo/is-touch-device]</span><span class="delimiter">: </span><span class="description">check if the current environment is a touch device.</span>
-   <span class="signature">[`IS_WEB_WORKER`][@taktikangea/blanditiis-nemo/is-web-worker]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web worker.</span>
-   <span class="signature">[`IS_WINDOWS`][@taktikangea/blanditiis-nemo/is-windows]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Windows.</span>

</div>

<!-- </toc> -->

To test whether a runtime environment supports certain features, the namespace includes the following utilities:

<!-- <toc pattern="has-*-support" > -->

<div class="namespace-toc">

-   <span class="signature">[`hasArrayBufferSupport()`][@taktikangea/blanditiis-nemo/has-arraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `ArrayBuffer` support.</span>
-   <span class="signature">[`hasArrowFunctionSupport()`][@taktikangea/blanditiis-nemo/has-arrow-function-support]</span><span class="delimiter">: </span><span class="description">detect native `arrow function` support.</span>
-   <span class="signature">[`hasAsyncAwaitSupport()`][@taktikangea/blanditiis-nemo/has-async-await-support]</span><span class="delimiter">: </span><span class="description">detect native `async`/`await` support.</span>
-   <span class="signature">[`hasAsyncIteratorSymbolSupport()`][@taktikangea/blanditiis-nemo/has-async-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.asyncIterator` support.</span>
-   <span class="signature">[`hasBigIntSupport()`][@taktikangea/blanditiis-nemo/has-bigint-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt` support.</span>
-   <span class="signature">[`hasBigInt64ArraySupport()`][@taktikangea/blanditiis-nemo/has-bigint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt64Array` support.</span>
-   <span class="signature">[`hasBigUint64ArraySupport()`][@taktikangea/blanditiis-nemo/has-biguint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigUint64Array` support.</span>
-   <span class="signature">[`hasClassSupport()`][@taktikangea/blanditiis-nemo/has-class-support]</span><span class="delimiter">: </span><span class="description">detect native `class` support.</span>
-   <span class="signature">[`hasDataViewSupport()`][@taktikangea/blanditiis-nemo/has-dataview-support]</span><span class="delimiter">: </span><span class="description">detect native `DataView` support.</span>
-   <span class="signature">[`hasDefinePropertiesSupport()`][@taktikangea/blanditiis-nemo/has-define-properties-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperties` support.</span>
-   <span class="signature">[`hasDefinePropertySupport()`][@taktikangea/blanditiis-nemo/has-define-property-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperty` support.</span>
-   <span class="signature">[`hasFloat32ArraySupport()`][@taktikangea/blanditiis-nemo/has-float32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float32Array` support.</span>
-   <span class="signature">[`hasFloat64ArraySupport()`][@taktikangea/blanditiis-nemo/has-float64array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float64Array` support.</span>
-   <span class="signature">[`hasFunctionNameSupport()`][@taktikangea/blanditiis-nemo/has-function-name-support]</span><span class="delimiter">: </span><span class="description">detect native function `name` support.</span>
-   <span class="signature">[`hasGeneratorSupport()`][@taktikangea/blanditiis-nemo/has-generator-support]</span><span class="delimiter">: </span><span class="description">detect native `generator function` support.</span>
-   <span class="signature">[`hasGlobalThisSupport()`][@taktikangea/blanditiis-nemo/has-globalthis-support]</span><span class="delimiter">: </span><span class="description">detect `globalThis` support.</span>
-   <span class="signature">[`hasInt16ArraySupport()`][@taktikangea/blanditiis-nemo/has-int16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int16Array` support.</span>
-   <span class="signature">[`hasInt32ArraySupport()`][@taktikangea/blanditiis-nemo/has-int32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int32Array` support.</span>
-   <span class="signature">[`hasInt8ArraySupport()`][@taktikangea/blanditiis-nemo/has-int8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int8Array` support.</span>
-   <span class="signature">[`hasIteratorSymbolSupport()`][@taktikangea/blanditiis-nemo/has-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.iterator` support.</span>
-   <span class="signature">[`hasMapSupport()`][@taktikangea/blanditiis-nemo/has-map-support]</span><span class="delimiter">: </span><span class="description">detect native `Map` support.</span>
-   <span class="signature">[`hasNodeBufferSupport()`][@taktikangea/blanditiis-nemo/has-node-buffer-support]</span><span class="delimiter">: </span><span class="description">detect native `Buffer` support.</span>
-   <span class="signature">[`hasProxySupport()`][@taktikangea/blanditiis-nemo/has-proxy-support]</span><span class="delimiter">: </span><span class="description">detect native `Proxy` support.</span>
-   <span class="signature">[`hasSetSupport()`][@taktikangea/blanditiis-nemo/has-set-support]</span><span class="delimiter">: </span><span class="description">detect native `Set` support.</span>
-   <span class="signature">[`hasSharedArrayBufferSupport()`][@taktikangea/blanditiis-nemo/has-sharedarraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `SharedArrayBuffer` support.</span>
-   <span class="signature">[`hasSymbolSupport()`][@taktikangea/blanditiis-nemo/has-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol` support.</span>
-   <span class="signature">[`hasToStringTagSupport()`][@taktikangea/blanditiis-nemo/has-tostringtag-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.toStringTag` support.</span>
-   <span class="signature">[`hasUint16ArraySupport()`][@taktikangea/blanditiis-nemo/has-uint16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint16Array` support.</span>
-   <span class="signature">[`hasUint32ArraySupport()`][@taktikangea/blanditiis-nemo/has-uint32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint32Array` support.</span>
-   <span class="signature">[`hasUint8ArraySupport()`][@taktikangea/blanditiis-nemo/has-uint8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8Array` support.</span>
-   <span class="signature">[`hasUint8ClampedArraySupport()`][@taktikangea/blanditiis-nemo/has-uint8clampedarray-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8ClampedArray` support.</span>
-   <span class="signature">[`hasWebAssemblySupport()`][@taktikangea/blanditiis-nemo/has-wasm-support]</span><span class="delimiter">: </span><span class="description">detect native WebAssembly support.</span>
-   <span class="signature">[`hasWeakMapSupport()`][@taktikangea/blanditiis-nemo/has-weakmap-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakMap` support.</span>
-   <span class="signature">[`hasWeakSetSupport()`][@taktikangea/blanditiis-nemo/has-weakset-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakSet` support.</span>

</div>

<!-- </toc> -->

The remaining namespace utilities are as follows:

<!-- <toc ignore="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" ignore="is-*+(number|integer)*" ignore="is-*array*" ignore="is-*error*" ignore="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|node|web-worker|windows)" ignore="has-*-support" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`contains( val, searchValue[, position] )`][@taktikangea/blanditiis-nemo/contains]</span><span class="delimiter">: </span><span class="description">test if an array-like value contains a search value.</span>
-   <span class="signature">[`deepEqual( a, b )`][@taktikangea/blanditiis-nemo/deep-equal]</span><span class="delimiter">: </span><span class="description">test for deep equality between two values.</span>
-   <span class="signature">[`deepHasOwnProp( value, path[, options] )`][@taktikangea/blanditiis-nemo/deep-has-own-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path.</span>
-   <span class="signature">[`deepHasProp( value, path[, options] )`][@taktikangea/blanditiis-nemo/deep-has-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path, either own or inherited.</span>
-   <span class="signature">[`hasOwnProp( value, property )`][@taktikangea/blanditiis-nemo/has-own-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property.</span>
-   <span class="signature">[`hasProp( value, property )`][@taktikangea/blanditiis-nemo/has-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property, either own or inherited.</span>
-   <span class="signature">[`hasUTF16SurrogatePairAt( string, position )`][@taktikangea/blanditiis-nemo/has-utf16-surrogate-pair-at]</span><span class="delimiter">: </span><span class="description">test if a position in a string marks the start of a UTF-16 surrogate pair.</span>
-   <span class="signature">[`instanceOf( value, constructor )`][@taktikangea/blanditiis-nemo/instance-of]</span><span class="delimiter">: </span><span class="description">test whether a value has in its prototype chain a specified constructor as a prototype property.</span>
-   <span class="signature">[`isAbsoluteHttpURI( value )`][@taktikangea/blanditiis-nemo/is-absolute-http-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute HTTP(S) URI.</span>
-   <span class="signature">[`isAbsolutePath( value )`][@taktikangea/blanditiis-nemo/is-absolute-path]</span><span class="delimiter">: </span><span class="description">test if a value is an absolute path.</span>
-   <span class="signature">[`isAbsoluteURI( value )`][@taktikangea/blanditiis-nemo/is-absolute-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute URI.</span>
-   <span class="signature">[`isAccessorPropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-accessor-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has an accessor descriptor.</span>
-   <span class="signature">[`isAccessorProperty( value, property )`][@taktikangea/blanditiis-nemo/is-accessor-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has an accessor descriptor.</span>
-   <span class="signature">[`isAlphagram( value )`][@taktikangea/blanditiis-nemo/is-alphagram]</span><span class="delimiter">: </span><span class="description">test if a value is an alphagram.</span>
-   <span class="signature">[`isAlphaNumeric( value )`][@taktikangea/blanditiis-nemo/is-alphanumeric]</span><span class="delimiter">: </span><span class="description">test whether a string contains only alphanumeric characters.</span>
-   <span class="signature">[`isAnagram( str, value )`][@taktikangea/blanditiis-nemo/is-anagram]</span><span class="delimiter">: </span><span class="description">test if a value is an anagram.</span>
-   <span class="signature">[`isArguments( value )`][@taktikangea/blanditiis-nemo/is-arguments]</span><span class="delimiter">: </span><span class="description">test if a value is an arguments object.</span>
-   <span class="signature">[`isArrowFunction( value )`][@taktikangea/blanditiis-nemo/is-arrow-function]</span><span class="delimiter">: </span><span class="description">test if a value is an `arrow function`.</span>
-   <span class="signature">[`isASCII( value )`][@taktikangea/blanditiis-nemo/is-ascii]</span><span class="delimiter">: </span><span class="description">test whether a character belongs to the ASCII character set and whether this is true for all characters in a provided string.</span>
-   <span class="signature">[`isBetween( value, a, b[, left, right] )`][@taktikangea/blanditiis-nemo/is-between]</span><span class="delimiter">: </span><span class="description">test if a value is between two values.</span>
-   <span class="signature">[`isBigInt( value )`][@taktikangea/blanditiis-nemo/is-bigint]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt.</span>
-   <span class="signature">[`isBinaryString( value )`][@taktikangea/blanditiis-nemo/is-binary-string]</span><span class="delimiter">: </span><span class="description">test if a value is a binary string.</span>
-   <span class="signature">[`isBlankString( value )`][@taktikangea/blanditiis-nemo/is-blank-string]</span><span class="delimiter">: </span><span class="description">test if a value is a blank string.</span>
-   <span class="signature">[`isBoxedPrimitive( value )`][@taktikangea/blanditiis-nemo/is-boxed-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript boxed primitive.</span>
-   <span class="signature">[`isBuffer( value )`][@taktikangea/blanditiis-nemo/is-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a Buffer object.</span>
-   <span class="signature">[`isCamelcase( value )`][@taktikangea/blanditiis-nemo/is-camelcase]</span><span class="delimiter">: </span><span class="description">test if a value is a camelcase string.</span>
-   <span class="signature">[`isCapitalized( value )`][@taktikangea/blanditiis-nemo/is-capitalized]</span><span class="delimiter">: </span><span class="description">test if a value is a string having an uppercase first character.</span>
-   <span class="signature">[`isCircular( value )`][@taktikangea/blanditiis-nemo/is-circular]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object containing a circular reference.</span>
-   <span class="signature">[`isCircular( value )`][@taktikangea/blanditiis-nemo/is-circular]</span><span class="delimiter">: </span><span class="description">test if an object-like value contains a circular reference.</span>
-   <span class="signature">[`isClass( value )`][@taktikangea/blanditiis-nemo/is-class]</span><span class="delimiter">: </span><span class="description">test if a value is a class.</span>
-   <span class="signature">[`isCollection( value )`][@taktikangea/blanditiis-nemo/is-collection]</span><span class="delimiter">: </span><span class="description">test if a value is a collection.</span>
-   <span class="signature">[`isComposite( value )`][@taktikangea/blanditiis-nemo/is-composite]</span><span class="delimiter">: </span><span class="description">test if a value is a composite number.</span>
-   <span class="signature">[`isConfigurablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-configurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is configurable.</span>
-   <span class="signature">[`isConfigurableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-configurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is configurable.</span>
-   <span class="signature">[`isConstantcase( value )`][@taktikangea/blanditiis-nemo/is-constantcase]</span><span class="delimiter">: </span><span class="description">test if a value is a constantcase string.</span>
-   <span class="signature">[`isCurrentYear( value )`][@taktikangea/blanditiis-nemo/is-current-year]</span><span class="delimiter">: </span><span class="description">test if a value is the current year.</span>
-   <span class="signature">[`isDataPropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-data-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has a data descriptor.</span>
-   <span class="signature">[`isDataProperty( value, property )`][@taktikangea/blanditiis-nemo/is-data-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has a data descriptor.</span>
-   <span class="signature">[`isDataView( value )`][@taktikangea/blanditiis-nemo/is-dataview]</span><span class="delimiter">: </span><span class="description">test if a value is a DataView.</span>
-   <span class="signature">[`isDigitString( value )`][@taktikangea/blanditiis-nemo/is-digit-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only numeric digits.</span>
-   <span class="signature">[`isDomainName( value )`][@taktikangea/blanditiis-nemo/is-domain-name]</span><span class="delimiter">: </span><span class="description">test if a value is a domain name.</span>
-   <span class="signature">[`isDurationString( value )`][@taktikangea/blanditiis-nemo/is-duration-string]</span><span class="delimiter">: </span><span class="description">test if a value is a duration string.</span>
-   <span class="signature">[`isEmailAddress( value )`][@taktikangea/blanditiis-nemo/is-email-address]</span><span class="delimiter">: </span><span class="description">test if a value is an email address.</span>
-   <span class="signature">[`isEmptyCollection( value )`][@taktikangea/blanditiis-nemo/is-empty-collection]</span><span class="delimiter">: </span><span class="description">test if a value is an empty collection.</span>
-   <span class="signature">[`isEmptyObject( value )`][@taktikangea/blanditiis-nemo/is-empty-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty object.</span>
-   <span class="signature">[`isEmptyString( value )`][@taktikangea/blanditiis-nemo/is-empty-string]</span><span class="delimiter">: </span><span class="description">test if a value is an empty string.</span>
-   <span class="signature">[`isEnumerablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-enumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is enumerable.</span>
-   <span class="signature">[`isEnumerableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-enumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is enumerable.</span>
-   <span class="signature">[`isEven( value )`][@taktikangea/blanditiis-nemo/is-even]</span><span class="delimiter">: </span><span class="description">test if a value is an even number.</span>
-   <span class="signature">[`isFalsy( value )`][@taktikangea/blanditiis-nemo/is-falsy]</span><span class="delimiter">: </span><span class="description">test if a value is falsy.</span>
-   <span class="signature">[`isFinite( value )`][@taktikangea/blanditiis-nemo/is-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a finite number.</span>
-   <span class="signature">[`isGeneratorObjectLike( value )`][@taktikangea/blanditiis-nemo/is-generator-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is `generator` object-like.</span>
-   <span class="signature">[`isGeneratorObject( value )`][@taktikangea/blanditiis-nemo/is-generator-object]</span><span class="delimiter">: </span><span class="description">test if a value is a `generator` object.</span>
-   <span class="signature">[`isgzipBuffer( value )`][@taktikangea/blanditiis-nemo/is-gzip-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a gzip buffer.</span>
-   <span class="signature">[`isHexString( value )`][@taktikangea/blanditiis-nemo/is-hex-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only hexadecimal digits.</span>
-   <span class="signature">[`isInfinite( value )`][@taktikangea/blanditiis-nemo/is-infinite]</span><span class="delimiter">: </span><span class="description">test if a value is an infinite number.</span>
-   <span class="signature">[`isInheritedProperty( value, property )`][@taktikangea/blanditiis-nemo/is-inherited-property]</span><span class="delimiter">: </span><span class="description">test if an object has an inherited property.</span>
-   <span class="signature">[`isIterableLike( value )`][@taktikangea/blanditiis-nemo/is-iterable-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterable`-like.</span>
-   <span class="signature">[`isIteratorLike( value )`][@taktikangea/blanditiis-nemo/is-iterator-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterator`-like.</span>
-   <span class="signature">[`isJSON( value )`][@taktikangea/blanditiis-nemo/is-json]</span><span class="delimiter">: </span><span class="description">test if a value is a parseable JSON string.</span>
-   <span class="signature">[`isKebabcase( value )`][@taktikangea/blanditiis-nemo/is-kebabcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in kebab case.</span>
-   <span class="signature">[`isLeapYear( [value] )`][@taktikangea/blanditiis-nemo/is-leap-year]</span><span class="delimiter">: </span><span class="description">test if a value corresponds to a leap year in the Gregorian calendar.</span>
-   <span class="signature">[`isLocalhost( value )`][@taktikangea/blanditiis-nemo/is-localhost]</span><span class="delimiter">: </span><span class="description">test whether a value is a localhost hostname.</span>
-   <span class="signature">[`isLowercase( value )`][@taktikangea/blanditiis-nemo/is-lowercase]</span><span class="delimiter">: </span><span class="description">test if a value is a lowercase string.</span>
-   <span class="signature">[`isMethodIn( value, property )`][@taktikangea/blanditiis-nemo/is-method-in]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name, either own or inherited.</span>
-   <span class="signature">[`isMethod( value, property )`][@taktikangea/blanditiis-nemo/is-method]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name.</span>
-   <span class="signature">[`isMultiSlice( value )`][@taktikangea/blanditiis-nemo/is-multi-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `MultiSlice`.</span>
-   <span class="signature">[`isNamedTypedTupleLike( value )`][@taktikangea/blanditiis-nemo/is-named-typed-tuple-like]</span><span class="delimiter">: </span><span class="description">test if a value is named typed tuple-like.</span>
-   <span class="signature">[`isNativeFunction( value )`][@taktikangea/blanditiis-nemo/is-native-function]</span><span class="delimiter">: </span><span class="description">test if a value is a native function.</span>
-   <span class="signature">[`isNegativeZero( value )`][@taktikangea/blanditiis-nemo/is-negative-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to negative zero.</span>
-   <span class="signature">[`isNodeBuiltin( value )`][@taktikangea/blanditiis-nemo/is-node-builtin]</span><span class="delimiter">: </span><span class="description">test whether a string matches a Node.js built-in module name.</span>
-   <span class="signature">[`isNodeDuplexStreamLike( value )`][@taktikangea/blanditiis-nemo/is-node-duplex-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node duplex stream-like.</span>
-   <span class="signature">[`isNodeReadableStreamLike( value )`][@taktikangea/blanditiis-nemo/is-node-readable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node readable stream-like.</span>
-   <span class="signature">[`isNodeREPL()`][@taktikangea/blanditiis-nemo/is-node-repl]</span><span class="delimiter">: </span><span class="description">check if running in a Node.js REPL environment.</span>
-   <span class="signature">[`isNodeStreamLike( value )`][@taktikangea/blanditiis-nemo/is-node-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node stream-like.</span>
-   <span class="signature">[`isNodeTransformStreamLike( value )`][@taktikangea/blanditiis-nemo/is-node-transform-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node transform stream-like.</span>
-   <span class="signature">[`isNodeWritableStreamLike( value )`][@taktikangea/blanditiis-nemo/is-node-writable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node writable stream-like.</span>
-   <span class="signature">[`isNonConfigurablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-nonconfigurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-configurable.</span>
-   <span class="signature">[`isNonConfigurableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-nonconfigurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-configurable.</span>
-   <span class="signature">[`isNonEnumerablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-nonenumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-enumerable.</span>
-   <span class="signature">[`isNonEnumerableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-nonenumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-enumerable.</span>
-   <span class="signature">[`isNonNegativeFinite( value )`][@taktikangea/blanditiis-nemo/is-nonnegative-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative finite value.</span>
-   <span class="signature">[`isObjectLike( value )`][@taktikangea/blanditiis-nemo/is-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is object-like.</span>
-   <span class="signature">[`isOdd( value )`][@taktikangea/blanditiis-nemo/is-odd]</span><span class="delimiter">: </span><span class="description">test if a value is an odd number.</span>
-   <span class="signature">[`isPascalcase( value )`][@taktikangea/blanditiis-nemo/is-pascalcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in Pascal case.</span>
-   <span class="signature">[`isPlainObject( value )`][@taktikangea/blanditiis-nemo/is-plain-object]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object.</span>
-   <span class="signature">[`isPositiveZero( value )`][@taktikangea/blanditiis-nemo/is-positive-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to positive zero.</span>
-   <span class="signature">[`isPrime( value )`][@taktikangea/blanditiis-nemo/is-prime]</span><span class="delimiter">: </span><span class="description">test if a value is a prime number.</span>
-   <span class="signature">[`isPrimitive( value )`][@taktikangea/blanditiis-nemo/is-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript primitive.</span>
-   <span class="signature">[`isPRNGLike( value )`][@taktikangea/blanditiis-nemo/is-prng-like]</span><span class="delimiter">: </span><span class="description">test if a value is PRNG-like.</span>
-   <span class="signature">[`isProbability( value )`][@taktikangea/blanditiis-nemo/is-probability]</span><span class="delimiter">: </span><span class="description">test if a value is a probability.</span>
-   <span class="signature">[`isPropertyKey( value )`][@taktikangea/blanditiis-nemo/is-property-key]</span><span class="delimiter">: </span><span class="description">test whether a value is a property key.</span>
-   <span class="signature">[`isPrototypeOf( obj, prototype )`][@taktikangea/blanditiis-nemo/is-prototype-of]</span><span class="delimiter">: </span><span class="description">test if an object's prototype chain contains a provided prototype.</span>
-   <span class="signature">[`isReadOnlyPropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-read-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is read-only.</span>
-   <span class="signature">[`isReadOnlyProperty( value, property )`][@taktikangea/blanditiis-nemo/is-read-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is read-only.</span>
-   <span class="signature">[`isReadWritePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-read-write-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable and writable.</span>
-   <span class="signature">[`isReadWriteProperty( value, property )`][@taktikangea/blanditiis-nemo/is-read-write-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable and writable.</span>
-   <span class="signature">[`isReadablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-readable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable.</span>
-   <span class="signature">[`isReadableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-readable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable.</span>
-   <span class="signature">[`isRegExpString( value )`][@taktikangea/blanditiis-nemo/is-regexp-string]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression string.</span>
-   <span class="signature">[`isRelativePath( value )`][@taktikangea/blanditiis-nemo/is-relative-path]</span><span class="delimiter">: </span><span class="description">test if a value is a relative path.</span>
-   <span class="signature">[`isRelativeURI( value )`][@taktikangea/blanditiis-nemo/is-relative-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is a relative URI.</span>
-   <span class="signature">[`isSameComplex128( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-complex128]</span><span class="delimiter">: </span><span class="description">test if two arguments are both double-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameComplex64( v1, v2 )`][@taktikangea/blanditiis-nemo/is-same-complex64]</span><span class="delimiter">: </span><span class="description">test if two arguments are both single-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameNativeClass( a, b )`][@taktikangea/blanditiis-nemo/is-same-native-class]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same native class.</span>
-   <span class="signature">[`isSameType( a, b )`][@taktikangea/blanditiis-nemo/is-same-type]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same type.</span>
-   <span class="signature">[`isSameValueZero( a, b )`][@taktikangea/blanditiis-nemo/is-same-value-zero]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSameValue( a, b )`][@taktikangea/blanditiis-nemo/is-same-value]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSemVer( value )`][@taktikangea/blanditiis-nemo/is-semver]</span><span class="delimiter">: </span><span class="description">test if a value is a semantic version string.</span>
-   <span class="signature">[`isSlice( value )`][@taktikangea/blanditiis-nemo/is-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `Slice`.</span>
-   <span class="signature">[`isSnakecase( value )`][@taktikangea/blanditiis-nemo/is-snakecase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in snake case.</span>
-   <span class="signature">[`isStartcase( value )`][@taktikangea/blanditiis-nemo/is-startcase]</span><span class="delimiter">: </span><span class="description">test if a value is a startcase string.</span>
-   <span class="signature">[`isStrictEqual( a, b )`][@taktikangea/blanditiis-nemo/is-strict-equal]</span><span class="delimiter">: </span><span class="description">test if two arguments are strictly equal.</span>
-   <span class="signature">[`isTruthy( value )`][@taktikangea/blanditiis-nemo/is-truthy]</span><span class="delimiter">: </span><span class="description">test if a value is truthy.</span>
-   <span class="signature">[`isUNCPath( value )`][@taktikangea/blanditiis-nemo/is-unc-path]</span><span class="delimiter">: </span><span class="description">test if a value is a UNC path.</span>
-   <span class="signature">[`isUndefinedOrNull( value )`][@taktikangea/blanditiis-nemo/is-undefined-or-null]</span><span class="delimiter">: </span><span class="description">test if a value is undefined or null.</span>
-   <span class="signature">[`isUppercase( value )`][@taktikangea/blanditiis-nemo/is-uppercase]</span><span class="delimiter">: </span><span class="description">test if a value is an uppercase string.</span>
-   <span class="signature">[`isURI( value )`][@taktikangea/blanditiis-nemo/is-uri]</span><span class="delimiter">: </span><span class="description">test if a value is a URI.</span>
-   <span class="signature">[`isWhitespace( value )`][@taktikangea/blanditiis-nemo/is-whitespace]</span><span class="delimiter">: </span><span class="description">test whether a string contains only white space characters.</span>
-   <span class="signature">[`isWritablePropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-writable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is writable.</span>
-   <span class="signature">[`isWritableProperty( value, property )`][@taktikangea/blanditiis-nemo/is-writable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is writable.</span>
-   <span class="signature">[`isWriteOnlyPropertyIn( value, property )`][@taktikangea/blanditiis-nemo/is-write-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is write-only.</span>
-   <span class="signature">[`isWriteOnlyProperty( value, property )`][@taktikangea/blanditiis-nemo/is-write-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is write-only.</span>
-   <span class="signature">[`tools`][@taktikangea/blanditiis-nemo/tools]</span><span class="delimiter">: </span><span class="description">assertion utility tools.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var assert = require( '@taktikangea/blanditiis-nemo' );

console.log( objectKeys( assert ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@taktikangea/blanditiis-nemo.svg
[npm-url]: https://npmjs.org/package/@taktikangea/blanditiis-nemo

[test-image]: https://github.com/taktikangea/blanditiis-nemo/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/taktikangea/blanditiis-nemo/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/taktikangea/blanditiis-nemo/main.svg
[coverage-url]: https://codecov.io/github/taktikangea/blanditiis-nemo?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/taktikangea/blanditiis-nemo.svg
[dependencies-url]: https://david-dm.org/taktikangea/blanditiis-nemo/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/taktikangea/blanditiis-nemo/tree/deno
[deno-readme]: https://github.com/taktikangea/blanditiis-nemo/blob/deno/README.md
[umd-url]: https://github.com/taktikangea/blanditiis-nemo/tree/umd
[umd-readme]: https://github.com/taktikangea/blanditiis-nemo/blob/umd/README.md
[esm-url]: https://github.com/taktikangea/blanditiis-nemo/tree/esm
[esm-readme]: https://github.com/taktikangea/blanditiis-nemo/blob/esm/README.md
[branches-url]: https://github.com/taktikangea/blanditiis-nemo/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/taktikangea/blanditiis-nemo/main/LICENSE

<!-- <toc-links> -->

[@taktikangea/blanditiis-nemo/contains]: https://github.com/taktikangea/blanditiis-nemo/tree/main/contains

[@taktikangea/blanditiis-nemo/deep-equal]: https://github.com/taktikangea/blanditiis-nemo/tree/main/deep-equal

[@taktikangea/blanditiis-nemo/deep-has-own-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/deep-has-own-property

[@taktikangea/blanditiis-nemo/deep-has-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/deep-has-property

[@taktikangea/blanditiis-nemo/has-own-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-own-property

[@taktikangea/blanditiis-nemo/has-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-property

[@taktikangea/blanditiis-nemo/has-utf16-surrogate-pair-at]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-utf16-surrogate-pair-at

[@taktikangea/blanditiis-nemo/instance-of]: https://github.com/taktikangea/blanditiis-nemo/tree/main/instance-of

[@taktikangea/blanditiis-nemo/is-absolute-http-uri]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-absolute-http-uri

[@taktikangea/blanditiis-nemo/is-absolute-path]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-absolute-path

[@taktikangea/blanditiis-nemo/is-absolute-uri]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-absolute-uri

[@taktikangea/blanditiis-nemo/is-accessor-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-accessor-property-in

[@taktikangea/blanditiis-nemo/is-accessor-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-accessor-property

[@taktikangea/blanditiis-nemo/is-alphagram]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-alphagram

[@taktikangea/blanditiis-nemo/is-alphanumeric]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-alphanumeric

[@taktikangea/blanditiis-nemo/is-anagram]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-anagram

[@taktikangea/blanditiis-nemo/is-arguments]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-arguments

[@taktikangea/blanditiis-nemo/is-arrow-function]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-arrow-function

[@taktikangea/blanditiis-nemo/is-ascii]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-ascii

[@taktikangea/blanditiis-nemo/is-between]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-between

[@taktikangea/blanditiis-nemo/is-bigint]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-bigint

[@taktikangea/blanditiis-nemo/is-binary-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-binary-string

[@taktikangea/blanditiis-nemo/is-blank-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-blank-string

[@taktikangea/blanditiis-nemo/is-boxed-primitive]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-boxed-primitive

[@taktikangea/blanditiis-nemo/is-buffer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-buffer

[@taktikangea/blanditiis-nemo/is-camelcase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-camelcase

[@taktikangea/blanditiis-nemo/is-capitalized]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-capitalized

[@taktikangea/blanditiis-nemo/is-circular]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-circular

[@taktikangea/blanditiis-nemo/is-class]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-class

[@taktikangea/blanditiis-nemo/is-collection]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-collection

[@taktikangea/blanditiis-nemo/is-composite]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-composite

[@taktikangea/blanditiis-nemo/is-configurable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-configurable-property-in

[@taktikangea/blanditiis-nemo/is-configurable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-configurable-property

[@taktikangea/blanditiis-nemo/is-constantcase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-constantcase

[@taktikangea/blanditiis-nemo/is-current-year]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-current-year

[@taktikangea/blanditiis-nemo/is-data-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-data-property-in

[@taktikangea/blanditiis-nemo/is-data-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-data-property

[@taktikangea/blanditiis-nemo/is-dataview]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-dataview

[@taktikangea/blanditiis-nemo/is-digit-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-digit-string

[@taktikangea/blanditiis-nemo/is-domain-name]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-domain-name

[@taktikangea/blanditiis-nemo/is-duration-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-duration-string

[@taktikangea/blanditiis-nemo/is-email-address]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-email-address

[@taktikangea/blanditiis-nemo/is-empty-collection]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-empty-collection

[@taktikangea/blanditiis-nemo/is-empty-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-empty-object

[@taktikangea/blanditiis-nemo/is-empty-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-empty-string

[@taktikangea/blanditiis-nemo/is-enumerable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-enumerable-property-in

[@taktikangea/blanditiis-nemo/is-enumerable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-enumerable-property

[@taktikangea/blanditiis-nemo/is-even]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-even

[@taktikangea/blanditiis-nemo/is-falsy]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-falsy

[@taktikangea/blanditiis-nemo/is-finite]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-finite

[@taktikangea/blanditiis-nemo/is-generator-object-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-generator-object-like

[@taktikangea/blanditiis-nemo/is-generator-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-generator-object

[@taktikangea/blanditiis-nemo/is-gzip-buffer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-gzip-buffer

[@taktikangea/blanditiis-nemo/is-hex-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-hex-string

[@taktikangea/blanditiis-nemo/is-infinite]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-infinite

[@taktikangea/blanditiis-nemo/is-inherited-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-inherited-property

[@taktikangea/blanditiis-nemo/is-iterable-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-iterable-like

[@taktikangea/blanditiis-nemo/is-iterator-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-iterator-like

[@taktikangea/blanditiis-nemo/is-json]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-json

[@taktikangea/blanditiis-nemo/is-kebabcase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-kebabcase

[@taktikangea/blanditiis-nemo/is-leap-year]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-leap-year

[@taktikangea/blanditiis-nemo/is-localhost]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-localhost

[@taktikangea/blanditiis-nemo/is-lowercase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-lowercase

[@taktikangea/blanditiis-nemo/is-method-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-method-in

[@taktikangea/blanditiis-nemo/is-method]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-method

[@taktikangea/blanditiis-nemo/is-multi-slice]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-multi-slice

[@taktikangea/blanditiis-nemo/is-named-typed-tuple-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-named-typed-tuple-like

[@taktikangea/blanditiis-nemo/is-native-function]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-native-function

[@taktikangea/blanditiis-nemo/is-negative-zero]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-negative-zero

[@taktikangea/blanditiis-nemo/is-node-builtin]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-builtin

[@taktikangea/blanditiis-nemo/is-node-duplex-stream-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-duplex-stream-like

[@taktikangea/blanditiis-nemo/is-node-readable-stream-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-readable-stream-like

[@taktikangea/blanditiis-nemo/is-node-repl]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-repl

[@taktikangea/blanditiis-nemo/is-node-stream-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-stream-like

[@taktikangea/blanditiis-nemo/is-node-transform-stream-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-transform-stream-like

[@taktikangea/blanditiis-nemo/is-node-writable-stream-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node-writable-stream-like

[@taktikangea/blanditiis-nemo/is-nonconfigurable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonconfigurable-property-in

[@taktikangea/blanditiis-nemo/is-nonconfigurable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonconfigurable-property

[@taktikangea/blanditiis-nemo/is-nonenumerable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonenumerable-property-in

[@taktikangea/blanditiis-nemo/is-nonenumerable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonenumerable-property

[@taktikangea/blanditiis-nemo/is-nonnegative-finite]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonnegative-finite

[@taktikangea/blanditiis-nemo/is-object-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-object-like

[@taktikangea/blanditiis-nemo/is-odd]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-odd

[@taktikangea/blanditiis-nemo/is-pascalcase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-pascalcase

[@taktikangea/blanditiis-nemo/is-plain-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-plain-object

[@taktikangea/blanditiis-nemo/is-positive-zero]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-positive-zero

[@taktikangea/blanditiis-nemo/is-prime]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-prime

[@taktikangea/blanditiis-nemo/is-primitive]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-primitive

[@taktikangea/blanditiis-nemo/is-prng-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-prng-like

[@taktikangea/blanditiis-nemo/is-probability]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-probability

[@taktikangea/blanditiis-nemo/is-property-key]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-property-key

[@taktikangea/blanditiis-nemo/is-prototype-of]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-prototype-of

[@taktikangea/blanditiis-nemo/is-read-only-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-read-only-property-in

[@taktikangea/blanditiis-nemo/is-read-only-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-read-only-property

[@taktikangea/blanditiis-nemo/is-read-write-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-read-write-property-in

[@taktikangea/blanditiis-nemo/is-read-write-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-read-write-property

[@taktikangea/blanditiis-nemo/is-readable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-readable-property-in

[@taktikangea/blanditiis-nemo/is-readable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-readable-property

[@taktikangea/blanditiis-nemo/is-regexp-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-regexp-string

[@taktikangea/blanditiis-nemo/is-relative-path]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-relative-path

[@taktikangea/blanditiis-nemo/is-relative-uri]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-relative-uri

[@taktikangea/blanditiis-nemo/is-same-complex128]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-complex128

[@taktikangea/blanditiis-nemo/is-same-complex64]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-complex64

[@taktikangea/blanditiis-nemo/is-same-native-class]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-native-class

[@taktikangea/blanditiis-nemo/is-same-type]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-type

[@taktikangea/blanditiis-nemo/is-same-value-zero]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-value-zero

[@taktikangea/blanditiis-nemo/is-same-value]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-value

[@taktikangea/blanditiis-nemo/is-semver]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-semver

[@taktikangea/blanditiis-nemo/is-slice]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-slice

[@taktikangea/blanditiis-nemo/is-snakecase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-snakecase

[@taktikangea/blanditiis-nemo/is-startcase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-startcase

[@taktikangea/blanditiis-nemo/is-strict-equal]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-strict-equal

[@taktikangea/blanditiis-nemo/is-truthy]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-truthy

[@taktikangea/blanditiis-nemo/is-unc-path]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-unc-path

[@taktikangea/blanditiis-nemo/is-undefined-or-null]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-undefined-or-null

[@taktikangea/blanditiis-nemo/is-uppercase]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uppercase

[@taktikangea/blanditiis-nemo/is-uri]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uri

[@taktikangea/blanditiis-nemo/is-whitespace]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-whitespace

[@taktikangea/blanditiis-nemo/is-writable-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-writable-property-in

[@taktikangea/blanditiis-nemo/is-writable-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-writable-property

[@taktikangea/blanditiis-nemo/is-write-only-property-in]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-write-only-property-in

[@taktikangea/blanditiis-nemo/is-write-only-property]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-write-only-property

[@taktikangea/blanditiis-nemo/tools]: https://github.com/taktikangea/blanditiis-nemo/tree/main/tools

[@taktikangea/blanditiis-nemo/has-arraybuffer-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-arraybuffer-support

[@taktikangea/blanditiis-nemo/has-arrow-function-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-arrow-function-support

[@taktikangea/blanditiis-nemo/has-async-await-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-async-await-support

[@taktikangea/blanditiis-nemo/has-async-iterator-symbol-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-async-iterator-symbol-support

[@taktikangea/blanditiis-nemo/has-bigint-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-bigint-support

[@taktikangea/blanditiis-nemo/has-bigint64array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-bigint64array-support

[@taktikangea/blanditiis-nemo/has-biguint64array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-biguint64array-support

[@taktikangea/blanditiis-nemo/has-class-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-class-support

[@taktikangea/blanditiis-nemo/has-dataview-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-dataview-support

[@taktikangea/blanditiis-nemo/has-define-properties-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-define-properties-support

[@taktikangea/blanditiis-nemo/has-define-property-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-define-property-support

[@taktikangea/blanditiis-nemo/has-float32array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-float32array-support

[@taktikangea/blanditiis-nemo/has-float64array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-float64array-support

[@taktikangea/blanditiis-nemo/has-function-name-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-function-name-support

[@taktikangea/blanditiis-nemo/has-generator-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-generator-support

[@taktikangea/blanditiis-nemo/has-globalthis-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-globalthis-support

[@taktikangea/blanditiis-nemo/has-int16array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-int16array-support

[@taktikangea/blanditiis-nemo/has-int32array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-int32array-support

[@taktikangea/blanditiis-nemo/has-int8array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-int8array-support

[@taktikangea/blanditiis-nemo/has-iterator-symbol-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-iterator-symbol-support

[@taktikangea/blanditiis-nemo/has-map-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-map-support

[@taktikangea/blanditiis-nemo/has-node-buffer-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-node-buffer-support

[@taktikangea/blanditiis-nemo/has-proxy-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-proxy-support

[@taktikangea/blanditiis-nemo/has-set-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-set-support

[@taktikangea/blanditiis-nemo/has-sharedarraybuffer-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-sharedarraybuffer-support

[@taktikangea/blanditiis-nemo/has-symbol-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-symbol-support

[@taktikangea/blanditiis-nemo/has-tostringtag-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-tostringtag-support

[@taktikangea/blanditiis-nemo/has-uint16array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-uint16array-support

[@taktikangea/blanditiis-nemo/has-uint32array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-uint32array-support

[@taktikangea/blanditiis-nemo/has-uint8array-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-uint8array-support

[@taktikangea/blanditiis-nemo/has-uint8clampedarray-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-uint8clampedarray-support

[@taktikangea/blanditiis-nemo/has-wasm-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-wasm-support

[@taktikangea/blanditiis-nemo/has-weakmap-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-weakmap-support

[@taktikangea/blanditiis-nemo/has-weakset-support]: https://github.com/taktikangea/blanditiis-nemo/tree/main/has-weakset-support

[@taktikangea/blanditiis-nemo/is-big-endian]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-big-endian

[@taktikangea/blanditiis-nemo/is-browser]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-browser

[@taktikangea/blanditiis-nemo/is-darwin]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-darwin

[@taktikangea/blanditiis-nemo/is-docker]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-docker

[@taktikangea/blanditiis-nemo/is-electron-main]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-electron-main

[@taktikangea/blanditiis-nemo/is-electron-renderer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-electron-renderer

[@taktikangea/blanditiis-nemo/is-electron]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-electron

[@taktikangea/blanditiis-nemo/is-little-endian]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-little-endian

[@taktikangea/blanditiis-nemo/is-mobile]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-mobile

[@taktikangea/blanditiis-nemo/is-node]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-node

[@taktikangea/blanditiis-nemo/is-touch-device]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-touch-device

[@taktikangea/blanditiis-nemo/is-web-worker]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-web-worker

[@taktikangea/blanditiis-nemo/is-windows]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-windows

[@taktikangea/blanditiis-nemo/is-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-error

[@taktikangea/blanditiis-nemo/is-eval-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-eval-error

[@taktikangea/blanditiis-nemo/is-range-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-range-error

[@taktikangea/blanditiis-nemo/is-reference-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-reference-error

[@taktikangea/blanditiis-nemo/is-syntax-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-syntax-error

[@taktikangea/blanditiis-nemo/is-type-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-type-error

[@taktikangea/blanditiis-nemo/is-uri-error]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uri-error

[@taktikangea/blanditiis-nemo/is-accessor-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-accessor-array

[@taktikangea/blanditiis-nemo/is-array-length]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-array-length

[@taktikangea/blanditiis-nemo/is-array-like-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-array-like-object

[@taktikangea/blanditiis-nemo/is-array-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-array-like

[@taktikangea/blanditiis-nemo/is-arraybuffer-view]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-arraybuffer-view

[@taktikangea/blanditiis-nemo/is-arraybuffer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-arraybuffer

[@taktikangea/blanditiis-nemo/is-between-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-between-array

[@taktikangea/blanditiis-nemo/is-bigint64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-bigint64array

[@taktikangea/blanditiis-nemo/is-biguint64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-biguint64array

[@taktikangea/blanditiis-nemo/is-circular-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-circular-array

[@taktikangea/blanditiis-nemo/is-empty-array-like-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-empty-array-like-object

[@taktikangea/blanditiis-nemo/is-empty-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-empty-array

[@taktikangea/blanditiis-nemo/is-falsy-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-falsy-array

[@taktikangea/blanditiis-nemo/is-finite-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-finite-array

[@taktikangea/blanditiis-nemo/is-numeric-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-numeric-array

[@taktikangea/blanditiis-nemo/is-plain-object-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-plain-object-array

[@taktikangea/blanditiis-nemo/is-probability-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-probability-array

[@taktikangea/blanditiis-nemo/is-same-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-array

[@taktikangea/blanditiis-nemo/is-same-complex128array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-complex128array

[@taktikangea/blanditiis-nemo/is-same-complex64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-complex64array

[@taktikangea/blanditiis-nemo/is-same-float32array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-float32array

[@taktikangea/blanditiis-nemo/is-same-float64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-same-float64array

[@taktikangea/blanditiis-nemo/is-sharedarraybuffer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-sharedarraybuffer

[@taktikangea/blanditiis-nemo/is-truthy-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-truthy-array

[@taktikangea/blanditiis-nemo/is-typed-array-length]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-typed-array-length

[@taktikangea/blanditiis-nemo/is-typed-array-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-typed-array-like

[@taktikangea/blanditiis-nemo/is-typed-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-typed-array

[@taktikangea/blanditiis-nemo/is-unity-probability-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-unity-probability-array

[@taktikangea/blanditiis-nemo/is-complex-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex-like

[@taktikangea/blanditiis-nemo/is-complex-typed-array-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex-typed-array-like

[@taktikangea/blanditiis-nemo/is-complex-typed-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex-typed-array

[@taktikangea/blanditiis-nemo/is-complex]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex

[@taktikangea/blanditiis-nemo/is-complex128]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex128

[@taktikangea/blanditiis-nemo/is-complex128array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex128array

[@taktikangea/blanditiis-nemo/is-complex64]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex64

[@taktikangea/blanditiis-nemo/is-complex64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex64array

[@taktikangea/blanditiis-nemo/is-centrosymmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-centrosymmetric-matrix

[@taktikangea/blanditiis-nemo/is-complex128matrix-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex128matrix-like

[@taktikangea/blanditiis-nemo/is-complex128ndarray-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex128ndarray-like

[@taktikangea/blanditiis-nemo/is-complex128vector-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex128vector-like

[@taktikangea/blanditiis-nemo/is-complex64matrix-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex64matrix-like

[@taktikangea/blanditiis-nemo/is-complex64ndarray-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex64ndarray-like

[@taktikangea/blanditiis-nemo/is-complex64vector-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-complex64vector-like

[@taktikangea/blanditiis-nemo/is-float32matrix-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float32matrix-like

[@taktikangea/blanditiis-nemo/is-float32ndarray-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float32ndarray-like

[@taktikangea/blanditiis-nemo/is-float32vector-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float32vector-like

[@taktikangea/blanditiis-nemo/is-float64matrix-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float64matrix-like

[@taktikangea/blanditiis-nemo/is-float64ndarray-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float64ndarray-like

[@taktikangea/blanditiis-nemo/is-float64vector-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float64vector-like

[@taktikangea/blanditiis-nemo/is-matrix-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-matrix-like

[@taktikangea/blanditiis-nemo/is-ndarray-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-ndarray-like

[@taktikangea/blanditiis-nemo/is-nonsymmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonsymmetric-matrix

[@taktikangea/blanditiis-nemo/is-persymmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-persymmetric-matrix

[@taktikangea/blanditiis-nemo/is-skew-centrosymmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-skew-centrosymmetric-matrix

[@taktikangea/blanditiis-nemo/is-skew-persymmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-skew-persymmetric-matrix

[@taktikangea/blanditiis-nemo/is-skew-symmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-skew-symmetric-matrix

[@taktikangea/blanditiis-nemo/is-square-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-square-matrix

[@taktikangea/blanditiis-nemo/is-symmetric-matrix]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-symmetric-matrix

[@taktikangea/blanditiis-nemo/is-vector-like]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-vector-like

[@taktikangea/blanditiis-nemo/is-float32array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float32array

[@taktikangea/blanditiis-nemo/is-float64array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-float64array

[@taktikangea/blanditiis-nemo/is-int16array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-int16array

[@taktikangea/blanditiis-nemo/is-int32array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-int32array

[@taktikangea/blanditiis-nemo/is-int8array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-int8array

[@taktikangea/blanditiis-nemo/is-uint16array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uint16array

[@taktikangea/blanditiis-nemo/is-uint32array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uint32array

[@taktikangea/blanditiis-nemo/is-uint8array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uint8array

[@taktikangea/blanditiis-nemo/is-uint8clampedarray]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-uint8clampedarray

[@taktikangea/blanditiis-nemo/is-cube-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-cube-number

[@taktikangea/blanditiis-nemo/is-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-integer-array

[@taktikangea/blanditiis-nemo/is-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-integer

[@taktikangea/blanditiis-nemo/is-negative-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-negative-integer-array

[@taktikangea/blanditiis-nemo/is-negative-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-negative-integer

[@taktikangea/blanditiis-nemo/is-negative-number-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-negative-number-array

[@taktikangea/blanditiis-nemo/is-negative-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-negative-number

[@taktikangea/blanditiis-nemo/is-nonnegative-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonnegative-integer-array

[@taktikangea/blanditiis-nemo/is-nonnegative-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonnegative-integer

[@taktikangea/blanditiis-nemo/is-nonnegative-number-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonnegative-number-array

[@taktikangea/blanditiis-nemo/is-nonnegative-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonnegative-number

[@taktikangea/blanditiis-nemo/is-nonpositive-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonpositive-integer-array

[@taktikangea/blanditiis-nemo/is-nonpositive-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonpositive-integer

[@taktikangea/blanditiis-nemo/is-nonpositive-number-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonpositive-number-array

[@taktikangea/blanditiis-nemo/is-nonpositive-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nonpositive-number

[@taktikangea/blanditiis-nemo/is-positive-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-positive-integer-array

[@taktikangea/blanditiis-nemo/is-positive-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-positive-integer

[@taktikangea/blanditiis-nemo/is-positive-number-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-positive-number-array

[@taktikangea/blanditiis-nemo/is-positive-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-positive-number

[@taktikangea/blanditiis-nemo/is-safe-integer-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-safe-integer-array

[@taktikangea/blanditiis-nemo/is-safe-integer]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-safe-integer

[@taktikangea/blanditiis-nemo/is-square-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-square-number

[@taktikangea/blanditiis-nemo/is-square-triangular-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-square-triangular-number

[@taktikangea/blanditiis-nemo/is-triangular-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-triangular-number

[@taktikangea/blanditiis-nemo/is-array-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-array-array

[@taktikangea/blanditiis-nemo/is-boolean-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-boolean-array

[@taktikangea/blanditiis-nemo/is-date-object-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-date-object-array

[@taktikangea/blanditiis-nemo/is-function-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-function-array

[@taktikangea/blanditiis-nemo/is-nan-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nan-array

[@taktikangea/blanditiis-nemo/is-null-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-null-array

[@taktikangea/blanditiis-nemo/is-number-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-number-array

[@taktikangea/blanditiis-nemo/is-object-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-object-array

[@taktikangea/blanditiis-nemo/is-string-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-string-array

[@taktikangea/blanditiis-nemo/is-symbol-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-symbol-array

[@taktikangea/blanditiis-nemo/is-array]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-array

[@taktikangea/blanditiis-nemo/is-boolean]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-boolean

[@taktikangea/blanditiis-nemo/is-date-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-date-object

[@taktikangea/blanditiis-nemo/is-function]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-function

[@taktikangea/blanditiis-nemo/is-nan]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-nan

[@taktikangea/blanditiis-nemo/is-null]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-null

[@taktikangea/blanditiis-nemo/is-number]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-number

[@taktikangea/blanditiis-nemo/is-object]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-object

[@taktikangea/blanditiis-nemo/is-regexp]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-regexp

[@taktikangea/blanditiis-nemo/is-string]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-string

[@taktikangea/blanditiis-nemo/is-symbol]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-symbol

[@taktikangea/blanditiis-nemo/is-undefined]: https://github.com/taktikangea/blanditiis-nemo/tree/main/is-undefined

<!-- </toc-links> -->

</section>

<!-- /.links -->
