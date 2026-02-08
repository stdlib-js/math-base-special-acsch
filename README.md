<!--

@license Apache-2.0

Copyright (c) 2022 The Stdlib Authors.

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

# acsch

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [hyperbolic arccosecant][inverse-hyperbolic-functions] of a number.



<section class="usage">

## Usage

```javascript
import acsch from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acsch@deno/mod.js';
```
The previous example will load the latest bundled code from the deno branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/math-base-special-acsch/tags). For example,

```javascript
import acsch from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acsch@v0.3.1-deno/mod.js';
```

#### acsch( x )

Computes the [hyperbolic arccosecant][inverse-hyperbolic-functions] of `x`.

```javascript
var v = acsch( 0.0 );
// returns Infinity

v = acsch( -0.0 );
// returns -Infinity

v = acsch( 1.0 );
// returns ~0.881

v = acsch( -1.0 );
// returns ~-0.881

v = acsch( NaN );
// returns NaN

v = acsch( -Infinity );
// returns -0.0

v = acsch( Infinity );
// returns 0.0
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import uniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-array-uniform@deno/mod.js';
import logEachMap from 'https://cdn.jsdelivr.net/gh/stdlib-js/console-log-each-map@deno/mod.js';
import acsch from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acsch@deno/mod.js';

var x = uniform( 100, 1.0, 5.0, {
    'dtype': 'float64'
});

logEachMap( 'acsch(%0.4f) = %0.4f', x, acsch );
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/acoth`][@stdlib/math/base/special/acoth]</span><span class="delimiter">: </span><span class="description">compute the inverse hyperbolic cotangent.</span>
-   <span class="package-name">[`@stdlib/math-base/special/acsc`][@stdlib/math/base/special/acsc]</span><span class="delimiter">: </span><span class="description">compute the arccosecant of a number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/asech`][@stdlib/math/base/special/asech]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arcsecant of a number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/asinh`][@stdlib/math/base/special/asinh]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arcsine of a double-precision floating-point number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/csc`][@stdlib/math/base/special/csc]</span><span class="delimiter">: </span><span class="description">compute the cosecant of a number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/csch`][@stdlib/math/base/special/csch]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic cosecant of a number.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2026. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-acsch.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-acsch

[test-image]: https://github.com/stdlib-js/math-base-special-acsch/actions/workflows/test.yml/badge.svg?branch=v0.3.1
[test-url]: https://github.com/stdlib-js/math-base-special-acsch/actions/workflows/test.yml?query=branch:v0.3.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-acsch/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-acsch?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-acsch.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-acsch/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-acsch/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-acsch/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-acsch/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-acsch/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-acsch/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-acsch/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-acsch/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-acsch/main/LICENSE

[inverse-hyperbolic-functions]: https://en.wikipedia.org/wiki/Inverse_hyperbolic_functions

<!-- <related-links> -->

[@stdlib/math/base/special/acoth]: https://github.com/stdlib-js/math-base-special-acoth/tree/deno

[@stdlib/math/base/special/acsc]: https://github.com/stdlib-js/math-base-special-acsc/tree/deno

[@stdlib/math/base/special/asech]: https://github.com/stdlib-js/math-base-special-asech/tree/deno

[@stdlib/math/base/special/asinh]: https://github.com/stdlib-js/math-base-special-asinh/tree/deno

[@stdlib/math/base/special/csc]: https://github.com/stdlib-js/math-base-special-csc/tree/deno

[@stdlib/math/base/special/csch]: https://github.com/stdlib-js/math-base-special-csch/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
