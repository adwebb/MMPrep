Part 1
======
Watch “Foundations of Programming: Fundamentals” at Lynda.com and then answer
the following questions:

1. Imagine asking a friend to meet you at a restaurant. What instructions would 
   a computer program need that your friend would not in order to understand how
   to get there?
   
The computer program would need a complete set of literal instructions, not referencing any landmarks or other things my friend may be familiar with, such as traffic laws. The computer program starts with no reference points other than the ones I give it. The computer will also follow the instructions precisely regardless of consequences, so it's more important that the instructions be absolutely correct.

2. What is the difference between source code and machine code? What does the
   CPU do? Where are instructions and data stored?
   
Source code is pseudo-english enough that we can easily read/parse it and determine what it's doing, much less write it ourselves. A compiler translates the source code it is given into Machine Code for a given CPU.  Machine code is largely unintelligible except to the CPU it is designed/compiled for. The CPU performs mathematical operations, so the machine code is a series of mathematical instructions that add up to accomplish what we asked for in the source code. Instructions and data are stored in the RAM while being processed.

3. What is an IDE and why is it useful?

Integrated Development Environments are useful because they include all of the benefits of a Programmer's Text Editor (such as automatic formatting/color-coding), as well as additional features, such as access to documentation and a built-in compiler. IDEs often offer templates which make building new programs easier, and have syntax-checking capability equivalent to spell-check to assist you in debugging your program.

4. What kind of a language is Objective-C? Why do you think we use it for making
   device specific applications? Why wouldn't we want to use an interpreted
   language for making iPhone and iPad apps?
   
As a compiled language, Objective-C is ideal for devices which have been designed to understand its compiled code, because it is ready to run and often faster. Using an interpreted language on devices such as an iPad or iPhone would be wasteful, forcing the device to work harder to interpret the source code in real-time. Particularly given mobile device limitations, we want to write software as device-specific as possible. 

Part Two
========
Read chapters *1* through *11* of The Big Nerd Ranch book and complete all the
exercises.
