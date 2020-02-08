# Eight

Sara Golemon

[Joind link](https://joind.in/talk/6155e)

PHP release manager

## PHP 8.0 - Newer versions are Better

Even minor releases have increases in speed/memory, which can save dollars.

### 7.0

* Twice as fast, half the memory
 * zval (fundamental storage unit in PHP) - changed from 32 to 16 bytes
* Scalar types
 * tiny bit of slowdown at runtime for type checking, but makes the code much more readable
* Anonymous Classes
* csprng - better random number generator
* Spaceship <=>
* Null coalesce ??
* EOL for over a year

### 7.1

* EOL over a month
* Scalar types, nullable
* List descructuring - syntactic sugar of list()
* HTTP/2 PUSH in curl

### 7.2

* 10% RPS throughput
* More scalar type hinting - Covarience/Contravarience
* Argon2i(d) password hashing
* libSodium crypto extension
* EOL at end of the year

### 7.3

* A bunch of small things

### 7.4

* Typed properties
* Arrow functions (closures)
* Bundle/Preload PHP code - Maybe don't use this yet
* WeakRefs
* Foreign Function Interface
* Digest availability
* Deprecations in prep for 8

### 8.0

* Coming out this Autumn-ish
* Union types (?string -> string|null)
* WeakMaps - Kick WeakRefs up a notch
* DOM "Living Standard" API
* Just In Time (JIT)
 * Memory and layout improvements already match HHVM for performance without a JIT
 * Initial experiments show _some_ real-world results
 * PHP exhibits bizarre behaviors
 * JIT lends itself to further optimications
 * (Call Forward Graph / Single Static Assignment)
 * (Inlining, Tail Recursion)
* Smaller features

### In the future?

* More typing? Generics?
* Retryables? (Maybe retry something if an exception was thrown)
* Comprehensions?
* Nullsafe Object Operator?
* Async/Await?