# Quantity over Quality

The headline is intentionally provocative but the idea is sound.
The only way to get good at doing a thing is to *do*  the thing.

Over, and over, and over...

# Clean Code chapter 1

Clean code is code that is easy to read, does one thing well and is well tested. Clean code doesn't happen by accident or all at once. Continuously make improvements, eack time leaving the code a little better than you left it.

# Red, Green, Refactor

* Write failing tests before writing code.
* Write the minimal code to make that test pass.
* Refactor that code (or the tests) and run tests again.
  * Make the tests more expressive
  * Make the test feedback reliable
  * Isolate tests
  * Make implementation code more expressive
  * Make implementation code more efficient
* Repeat

# TDD Cycles

There are multiple cycles of TDD: Nano, Micro, Milli, and Primary 

## Nano Cycle
This is the second by second cycle, the smallest building block that the other cycles rely upon.
1. Write a failing test before writing any code
1. The test should be the minimal amount of code to fail or fail to compile
1. Write the minimal amount of code ot pass the test

## Micro Cycle
Once you have the nano-scale pieces working combine them into unit tests.

1. Create a unit test that fails
1. Write production code that makes that test pass.
1. Clean up the mess you just made.

Make it work, make it right, make it fast.

## Milli Cycle
This cycle is where the code becomes useful in addition to passing tests. At this stage code should be becoming more generalized. Generalized code will pass tests with more parameters. As Volkswagen showed, writing software with the sole purpose of passing tests can lead to unwanted results.

## Primary Cycle
Look at the whole system, does the component you're working on affect other areas of the system? Where are the lines between components of the system, how do they affect one another.

