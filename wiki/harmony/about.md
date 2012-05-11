# About Harmony

TC39 uses what it calls the "Harmony" process for standardizing JavaScript. Individuals or small groups work as *champions* of a feature, and do design work independently of the rest of the group. When their design is ready for initial review, they create a [strawman](/strawman) proposal. Strawmen that are considered valuable are considered to have achieved *harmony*, at which point they are promoted to a [harmony](/harmony) proposal and worked on further. Harmony proposals are not guaranteed to be accepted in the language. They indicate that the group has consensus on the general approach of the proposal. But they still require more work in order to make *final* status, at which point they become part of the standard.

## Goals

These goals were agreed on at a meeting in July, 2008:

  1. Be a better language for writing:
    * complex applications;
    * libraries (possibly including the DOM) shared by those applications;
    * code generators targeting the new edition.
  1. Switch to a testable specification, ideally a definitional interpreter hosted mostly in ES5.
  1. Improve interoperation, adopting *de facto* standards where possible.
  1. Keep versioning as simple and linear as possible.
  1. Support a statically verifiable, object-capability secure subset.

## Means

  1. Minimize the additional semantic state needed beyond ES5.
  1. Provide syntactic convenience:
    * for good abstraction patterns;
    * for high integrity patterns;
    * defined by desugaring into kernel semantics.
  1. Remove (via opt-in versioning or pragmas) confusing or troublesome constructs.
    * Harmony builds on ES5 strict mode to avoid too many modes.
  1. Support virtualizability, allowing for host object emulation.

## Themes

  1. Modularity, or how to delineate units of source code to hide the insides from outside users
  1. Isolation, to prevent effects from propagating, or allow them only through certain references
    * Zero-authority maker-style modules
    * Other combinations of primordials/contexts/builtins with modules
    * Lack of isolation in browsers: multiple connected global objects
  1. Virtualization, for stratified guest code hosting, bridging disjoint object systems, and in particular emulating host objects
    * Proxies
    * Weak references or Ephemerons
  1. Control Effects, for simpler iteration and state-machine code
    * Delimited continuations
    * Generators, iterators
  1. Library/Tool Enabling, so the TC39 committee is not blocking library evolution
    * Object.hashcode
    * Byte arrays of some kind
    * Value types (for Decimal, etc.).
  1. Language Reform, the “better carrots” needed to lead users away from bad forms
    * let, const, function in block scope
    * Default and rest parameters, the spread operator
    * Destructuring
  1. Versioning, since new syntax is part of Harmony.
    * This theme is about minimizing opt-in versioning, easing migration, and future-proofing for the next edition.

