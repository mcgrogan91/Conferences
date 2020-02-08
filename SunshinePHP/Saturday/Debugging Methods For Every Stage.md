# The Fault In Our Code: Debugging Methods For Every Stage

Camilo Payan

[@cpayan_](https://twitter.com/cpayan_)

[Joind link](https://joind.in/talk/96324)

## Acceptance - the first step

We're all imperfect humans in an imperfect world, and will keep creating new bugs

There's no magic bullet for bugs.  There's power in consistency.

## Steps

### Step 0: Understand the system

Includes:
* Your codebase
* How PHP works
* How HTTP works
* How your database works

You gain this knowledge by reading.  A lot.  Manuals, code (yours, vendors, library), documentation.

### Step 1: Make it fail.  A lot

A repeatable set of steps to reproduce the bug.  Write those down.  This can help you automate the failure.

Understanding your system is important so you know what the expected behavior is.

_Suggestion_: Write the reproducable in Gherkin

Ensure your environment is similar to where the error occurred:
* Vagrant
* Docker
* QA Server

#### Wrong way to debug
1. Fill list from slide deck later

Do just enough thinking to narrow down where you might look, then just start looking for proof.