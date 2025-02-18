# Alternative Interpreters

## JavaScript

See [javascript.md](javascript.md) - work in progress.

## PHP

### Alternative interpreters and compilers

* [php-wasm](https://github.com/seanmorris/php-wasm) - Run PHP right in the browser. Live demo included.
* [ePHP](https://github.com/bragful/ephp) - PHP Interpreter in pure 100% Erlang (requires Erlang/OTP 19+), see [compatibility table](https://github.com/bragful/ephp/blob/master/doc/COMPATIBILITY.md)
* [graalphp](https://github.com/abertschi/graalphp) - an experimental just-in-time (JIT) compiler and runtime for PHP 7.4+ built on [GraalVM](https://www.graalvm.org/22.2/docs/introduction/) (see some [benchmarks](https://github.com/abertschi/graalphp/blob/master/results.md))
* [Goro](https://github.com/MagicalTux/goro) - incomplete implementation of PHP 7.2 written in pure [Go](https://go.dev/) with support for [goroutines](https://golangbot.com/goroutines/), better caching of compiled code by allowing sharing of compiled or live objects (classes, objects, etc) between running PHP scripts
* [HippyVM](https://github.com/hippyvm/hippyvm) - an implementation of the PHP language using RPython/PyPy technology
* [JPHP](https://github.com/jphp-group/jphp) - compiles PHP 7.1+ sources to JVM bytecode which can be executed on Java VM; adds possibility to use Java libraries in PHP, Java-like multithreading, sockets, creating GUI Android and Desktop apps (JavaFX or SWT), hot reloading for classes and functions; offers dedicated IDE called [DevelNext IDE](https://github.com/jphp-group/develnext-ide)
* [KPHP](https://vkcom.github.io/kphp/) - compiles a limited subset of PHP to a native binary running faster than PHP
* [PeachPie](https://www.peachpie.io/) - a modern PHP compiler based on the [Microsoft Roslyn](https://github.com/dotnet/roslyn) compiler platform and drawing from [Phalanger](https://github.com/DEVSENSE/Phalanger) project (PHP 5.4 compiler for .NET/Mono); it allows PHP to be executed within the .NET framework, thereby opening the door for PHP developers into the world of .NET and vice versa.
* [php.js](http://phpjs.hertzen.com/) -  reads PHP code and transforms it into JavaScript code and then runs
* [PH7](https://ph7.symisc.net/) - An Embedded Implementation of PHP 5 with a lot of PHP 7+ and C++-like improvements, see its [distinctive features](https://ph7.symisc.net/features.html)
* [pipp](https://github.com/RemiWoler/pipp) - an implementation of the language PHP that runs on [Parrot Virtual Machine](https://github.com/parrot/parrot), predeccessor of [MoarVM](https://github.com/MoarVM/MoarVM)
* [PolarPHP](https://github.com/polarphp/polarphp) - PHP 7 compiler with support for asynchronous programming, multi-threading and coroutines
* [pyhp](https://github.com/juokaz/pyhp) - incomplete implementation of the PHP language using the RPython technology (for complete implementation see: HippyVM)
* [pyhp.js](https://github.com/juokaz/pyhp.js) - PyHP interpreter translated into JavaScript using emscripten, resulting javascript file is asm.js which can be loaded in any browser or ran with Node.js
* [Quercus](https://www.caucho.com/resin-3.1/doc/quercus.xtp) - Java implementation of the PHP language
* [PHPPHP](https://github.com/ircmaxell/PHPPHP) - PHP interpreter written in PHP, low performance, predecessor of much faster Recki Compiler Toolkit for PHP
* [Recki Compiler Toolkit for PHP](https://github.com/google/recki-ct) - quote from [1]: "a compiler written entirely in PHP and only targets a subset of the PHP specification. It intentionally limits itself to a more static subset so that it is faster. This means that it does not support things like references, variable-variables and global variables. Recki-CT compiles PHP down to machine code but unlike HHVM and HippyVM, which use Just in Time compilation to compile PHP, it uses Ahead of Time compilation which caches an intermediary representation that can be compiled at run-time. Therefore, more aggressive optimisations can be applied and more efficient code can be generated. Based on trivial benchmarks, Recki-CT proves to be extremely fast."
* [php-compiler](https://github.com/ircmaxell/php-compiler) - PHP compiler, succesor of PHPPHP and Recki Compiler Toolkit for PHP
* [Uniter](https://phptojs.com/) - PHP client-side in the browser or in Node.js.

Referenced in academic papers but not located online:

* P8 - a Java implementation of PHP 5 with Java bytecode generation,  running on IBM J9 VM 1.5.0, referenced in [4]
* P9 - a JIT-compiler-based PHP engine, based on IBM J9 VM 1.5.0, referenced in [4]

Some old stuff: https://stackoverflow.com/a/1408499/925196

### Trans-compilers

* [Blueberry](https://github.com/gosukiwi/Blueberry) - a script language with clean syntax, inspired from Ruby, CoffeeScript, and Python which compiles to PHP
* [Fructose](https://github.com/haileys/Fructose) - a Ruby-like language that compiles to PHP
* [Haxe](https://haxe.org/) - high-level strictly-typed programming language with a fast optimizing cross-compiler which also compiles to PHP
* [mammouth](https://github.com/btwael/mammouth) - a small language that compiles into PHP, inspired by CoffeeScript (eg. "Everything is an expression"); compiler itself is written in Dart
* [Phabel](https://github.com/phabelio/phabel) - allows native usage of PHP 8+ features and especially syntax in projects and libraries, while allowing maintainers to publish a version targeting lower versions of php
* [Pharen](https://github.com/scriptor/pharen) - compiles a Lisp-inspired language to PHP
* [Phel](https://phel-lang.org/) - dialect of Lisp that compiles to PHP
* [Pratphall](http://cretz.github.io/pratphall/) - an optionally-typed language that compiles to readable PHP
* [Salty](https://github.com/egonschiele/salty) - a language that compiles to PHP, JavaScript, and JSX; Haskell-inspired
* [Snowscript](https://github.com/runekaagaard/snowscript) - a language that compiles to PHP; its syntax is inspired by Python, Lua, Coffescript, Go and Scala and strives to be DRY, clean and easy to read as well as write
* [THT](https://tht.dev/) - a clean re-design of PHP, making it more secure and easier to use; see [how THT compares to PHP](https://tht.dev/about/how-tht-compares-to-php)
* [tré](https://github.com/SvenMichaelKlose/tre) - transpiles Lisp to JavaScript and PHP7+; runs on top of Steel Bank Common Lisp (sbcl).
* [XP Compiler](https://github.com/xp-framework/compiler) - translates between Hack language, PHP 8.2, 8.1, 8.0, PHP 7.4, PHP 7.3, PHP 7.2, PHP 7.1 and PHP 7.0.

Also transcompilers not for full programming languages:

* [Swagger Editor](https://editor.swagger.io/) - can generate PHP client code from OpenAPI JSON description
* [Twig](https://twig.symfony.com/) - a templating engine and language that compiles to PHP;

### Preprocessors

* [Pre](https://github.com/preprocess) - compiles new syntax to work in new and old versions of PHP; original website of this project is down, but it's code is avalable in [this GitHub repo](https://github.com/preprocess/preprocess.io). Still, its might be better to check all the different repos available for the user ["Pre."](https://github.com/preprocess) as they seem to be different preprocessors built on top of some shared library or framework (see [this list of packages dependent on pre/plugin](https://packagist.org/packages/pre/plugin/dependents?order_by=downloads))

### Alternative PHP Virtual Machines

* [HHVM](https://hhvm.com/) - an open-source virtual machine designed for executing programs written in [Hack](https://hacklang.org/) (originally superset of PHP)
* [Tagua VM](https://github.com/tagua-vm/tagua-vm) - an experimental PHP Virtual Machine that guarantees safety and quality by removing large classes of vulnerabilities thanks to the Rust language and the LLVM Compiler Infrastructure

### Other

* [AerScript](https://github.com/sc0ttj/AerScript) - general-purpose, object-oriented scripting programming language based on PH7 (alternative PHP interpreter)

### Languages derived from PHP

* [Hack](https://hacklang.org/) - PHP-like new language with gradual typing, generics and new container types (vector, map, set, pair) executed on HipHop Virtual Machine (HHVM) [2][6]

### Research papers

#### References

* [1] KHAN, Sher Ali; MAFFEIS, Sergio. A Comparative Study of PHP Dialects. 2015.
* [2] ADAMS, Keith, et al. The hiphop virtual machine. In: Proceedings of the 2014 ACM International Conference on Object Oriented Programming Systems Languages & Applications. 2014. p. 777-790.
* [3] OTTONI, Guilherme. HHVM JIT: A Profile-guided, Region-based Compiler for PHP and Hack. In: Proceedings of the 39th ACM SIGPLAN Conference on Programming Language Design and Implementation. 2018. p. 151-165.
* [4] TATSUBORI, Michiaki, et al. Evaluation of a just-in-time compiler retrofitted for PHP. ACM Sigplan Notices, 2010, 45.7: 121-132.
* [5] BENDA, Jan; MATOUSEK, Tomas; PROSEK, Ladislav. Phalanger: Compiling and running PHP applications on the Microsoft .NET platform. .NET Technologies 2006, 2006.
* [6] ZHAO, Haiping, et al. The HipHop compiler for PHP. ACM SIGPLAN Notices, 2012, 47.10: 575-586.
