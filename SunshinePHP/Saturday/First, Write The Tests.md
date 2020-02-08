
# First, Write The Tests

Bryce Embry

[Joind link](https://joind.in/talk/cd26a)

Journey from not writing tests, to TDD

## The journey

Woodworking analogy:
* First wood box he made was awkward, joints had lots of gaps
* Sketched out a table, didn't use proper tools, it's _wobbly_

## As a developer

### First step

* Initial job, hiring manager said "We don't write tests".
* Testing by manually pushing buttons/etc
* Sometimes it takes 52 screens or to set up a test
* If you find yourself doing the same thing over and over again, that's a sign you need to write code
* Manual tests are hard.  So many permutations!
* Outsources testing to users. Poor user experience
* Wobbly PHP developer

### Getting into testing

* Hard to know where to start
  * What engine?
  * How do I test long methods? - You don't, you break them down
* What exactly am I testing, again?
  * Testing to clarify uncertainty
  * Testing to Generate Templates
  * "Does it crash" tests
* QA was still catching a lot of the problems
* Pragmatic testing - just writing the tests you think you need

### Trying TDD

* Painful at first
* Forced to think ahead
 * It's really hard to just move stuff around
 * Prevented accidental code duplication
* Writing code is more like writing english than math
  * You have your outline, and plan the paper, etc
* Provided a template to follow by writing out the scenarios
* Provided a safety net during refactors of active development
* Protected against breaking changes


## Conclusion
You can write without tests, like you can woodwork without proper tools and planning.  But it'll show.