# LunarML

A Standard ML compiler that produces Lua.

## Building

You need a recent version of MLton to build the executable, and Lua 5.3+ to run the compiled script.

```
$ make
$ make test
$ ./lunarml example/hello.sml
$ lua example/hello.lua
Hello world!
```

## Features

* [A subset of SML Basis Library](BasisLibrary.md)
* [Interface to Lua](LuaInterface.md)

The following SML '97 features are not implemented yet:

* `abstype`
* Signatures
    * Work in progress
* Functors

Successor ML features:

* [x] Monomorphic non-exhaustive bindings
* [x] Simplified recursive value bindings
    * SML '97-compatible declaration for type variables are also supported: `val <tyvarseq> rec <valbind>`
* [ ] Abstype as derived form
* [x] Fixed manifest type specifications
* [x] Abolish sequenced type realizations
* [ ] Line comments
* [ ] Extended literal syntax
* [ ] Record punning
* [ ] Record extension
* [ ] Record update
* [ ] Conjunctive patterns
* [ ] Nested matches
* [ ] Pattern guards
* [ ] Optional bars and semicolons
* [ ] Optional else branch
* [ ] Do declarations
* [x] Withtype in signatures

Other extensions planned:

* [x] Vector expressions and patterns
* [ ] Packaged modules (like in Alice ML or HaMLet S)
* [ ] Hexadecimal floating-point literals
* [ ] Variably-encoded Unicode escape sequence in string literals
