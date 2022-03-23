##  Testing
Unit tests verify the most basic functionality of your code, thus safeguarding against bugs introduced in refactoring.
 Unit tests don’t deal with their environment and with external systems to the codebase.
 If it you’ve written something that can fail when run on a machine without the “proper setup,” you haven’t written a unit test.
 unit tests don’t exercise multiple components of your system and how they act.  If you have a console application and you pipe input to it from the command line and test for output, you’re executing an end-to-end system test — not a unit test.

## Documentation
 In addition to assisting with refactoring, unit tests serve as vital documentation for fellow programmers
 You may also have an external documentation directory with examples of how to run your project, or perhaps you have been writing comments within your code to best communicate with your teammates about your changes.

 ## README
One of the most crucial things in your open source project is the README.md file
Whether the programmer will start building a program from scratch or will modify a program that another programmer has built, he needs to README badly, without him he will be like a wanderer and he will not know where to start or what to do