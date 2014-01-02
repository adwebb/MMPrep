Challenge 3: Get Your Hands Dirty
=================================
Next up, find the Lynda.com video series entitled: “Objective-C Essential
Training”. Watch each video in the following list and answer the corresponding
question.

Section 1: Getting Started
==========================
[1.1] Installing the tools (4:42)
---------------------------------
You should already have Xcode installed, but you will need to register as an
Apple Developer.

Do you like cats?

**ANSWER HERE**<>I do! I have two dogs that think they are cats. One is more convincing than the other.<>

[1.2] Creating your first application (11:28)
---------------------------------------------
Create your first application using the same steps Simon describes in the video.
Familiarize yourself with the Xcode environment, specifically notice how it can
be manipulated to display different helper tools and how it will attempt to fill
in your code as you type it.

**DO YOU PROMISE YOU DID IT?**<>I do so promise.<>

[1.3] Updates to this course (3:31)
-----------------------------------
Why do you think it's important to be aware of the idiosyncracies with older
versions of Objective-C and to keep up with new features as they are added?

**ANSWER HERE, IF YOU DARE…**<>I was totally watching the 2013 version until I realized 1.3 didn't match. It's important to be passingly familiar with the old way of doing things so that it doesn't confuse us when we run across it. It's important to keep up with new features because, by and large, the new features are being made for ease-of-use purposes.<>

Section 2: Objective-C Basics
=============================
[2.1] The Objective-C language (4:11)
-------------------------------------
How did Objective-C become the language to learn if you want to make apps for
the iPhone and iPad?

**ANSWER HERE**<>NeXT, founded by Steve Jobs after he left Apple, used Objective-C to make their NeXTStep OS. When NeXT was bought by Apple in 1996, they used NeXTStep to create OSX.  NS stands for NeXTStep. OSX was then used to build iOS.<>

[2.2] The structure of an Objective-C program (6:15)
----------------------------------------------------
Create a new project. Go to the menu option `Xcode`, `Preferences`,
`Text Editing` and make sure *Line Numbers* is checked in the section marked
"Show." Then add comments describing the purpose of each auto-generated line in
the main.m file. For example on Line 17 I would write: 

```
NSLog(@"Hello, World!");  // instructs the console to output: Hello, World!
```
<>#import <Foundation/Foundation.h> //the following code can utilize everything contained within the foundation framework header

int main(int argc, const char * argv[]) // this is the main function of the program
{ //main function begins

    @autoreleasepool { //ensures we don't have a memory leak
        
        // insert code here...
        NSLog(@"Hello, World!"); //prints "Hello, World!" on the screen.
        
    } //frees up the memory block(s) the above code required
    return 0; //program finished
} //main function ends<>

[2.3] Compiling and running your code (8:37)
--------------------------------------------
Why might you build in one version of iOS but deploy in an older version?

**ANSWER HERE**<>You want to build with all of the newest features being possible and supported, but also allow for users with older devices to use your program, even if the functionality is limited by their device.<>



Section 3: Program Flow
=======================
[3.1] Logging messages to the command line (6:07)
-------------------------------------------------
Following the example in the video, write a program that calculates and outputs
to the console the number of seconds in ten years. Copy and paste your code
here.

**PASTE HERE**<>#import <Foundation/Foundation.h>

int main(int argc, const char * argv[])
{

    @autoreleasepool {
        
        // insert code here...
        
        int seconds = 60; //number of seconds in a minute
        int minutes = 60; //number of minutes in an hour
        int hours = 24;   //number of hours in a day
        int days = 365;   //number of days in a year
        
        int secondsInTen = 10 * seconds * minutes * hours * days; //calculates seconds in 10 years
        
        NSLog(@"There are %i seconds in a decade.",secondsInTen); //outputs results
        
    }
    return 0;
}<>

[3.2] Writing conditional code (7:01)
-------------------------------------
Using Objective-C, create an integer variable called "day" that represents the
days of the week. Write an if statement that checks whether "day" is a weekend
day. If the day is a weekend day then have your program print a message saying
"Have a nice weekend!" and if it's not, print a message saying "I hope you're
having a good week!"

**PASTE HERE**<>
int day = 2; //a value of 0-6 corresponding to sunday-saturday.
        
        if(day == 0 || day == 6){ //checks if the day is saturday or sunday
            NSLog(@"Have a nice weekend!"); //wishes the user a nice weekend if it is
        } else{ //if it is not...
            NSLog(@"I hope you're having a good week!"); //wishes them a nice week.
		}
<>

[3.3] The switch statement (5:58)
---------------------------------
Create a variable called "hurricaneCategory" and a switch statement that prints
out a message describing a hurricane's category from 1-5.

**PASTE HERE**<>Couldn't this just be done with a 
NSLog(@"Yep, looks like a Category %i Hurricane to me. Sorry pal, you'd better run!",hurricaneCategory);? 

int hurricaneCategory = 10;

switch (hurricaneCategory) {
            case 1:
                NSLog(@"There appears to be a Category 1 Hurricane headed your direction. This indicates winds in excess of 74 MPH. Very dangerous winds will produce some damage: Well-constructed frame homes could have damage to roof, shingles, vinyl siding and gutters. Large branches of trees will snap and shallowly rooted trees may be toppled. Extensive damage to power lines and poles likely will result in power outages that could last a few to several days.");
                break;
            case 2:
                NSLog(@"There appears to be a Category 2 Hurricane headed your direction. This indicates winds in excess of 95 MPH. Extremely dangerous winds will cause extensive damage: Well-constructed frame homes could sustain major roof and siding damage. Many shallowly rooted trees will be snapped or uprooted and block numerous roads. Near-total power loss is expected with outages that could last from several days to weeks.");
            case 3:
                NSLog(@"There appears to be a Category 3 Hurricane headed your direction. This indicates winds in excess of 110 MPH. Devastating damage will occur: Well-built framed homes may incur major damage or removal of roof decking and gable ends. Many trees will be snapped or uprooted, blocking numerous roads. Electricity and water will be unavailable for several days to weeks after the storm passes.");
            case 4:
                NSLog(@"There appears to be a Category 4 Hurricane headed your direction. This indicates winds in excess of 130 MPH. Catastrophic damage will occur: Well-built framed homes can sustain severe damage with loss of most of the roof structure and/or some exterior walls. Most trees will be snapped or uprooted and power poles downed. Fallen trees and power poles will isolate residential areas. Power outages will last weeks to possibly months. Most of the area will be uninhabitable for weeks or months.");
            case 5:
                NSLog(@"There appears to be a Category 5 Hurricane headed your direction. This indicates winds in excess of 156 MPH. Catastrophic damage will occur: A high percentage of framed homes will be destroyed, with total roof failure and wall collapse. Fallen trees and power poles will isolate residential areas. Power outages will last for weeks to possibly months. Most of the area will be uninhabitable for weeks or months.");
                
            default:
                NSLog(@"I don't know what's coming at you, but it doesn't appear to be a Hurricane. I suggest running.");
                break;
        }


  
  
<>

[3.4] Code snippets (5:15)
--------------------------
Grab a code snippet, indent it to match the indent of your project, then add
comments to it, then select the entire snippet you just modified and save it as
your own code snippet. Time yourself and record how many seconds it takes you to
do all this.

**IT TOOK ME [52] SECONDS**

[3.5] Operators and expressions (11:08)
---------------------------------------
List the 6 types of operators described in this video. Provide their name, a
description of their meaning, and the syntax you would use to execute them. What
code snippet does the ternary operator replace?

**ANSWER HERE**<>
Arithmetic Operators: + - * / =  These work much as expected, with the exception that the result is always to the left of the equals sign. There are shortcut operators for +=, -=, *=, and /=, which take the existing value of the variable we are operating on and add, subtract, multiply, or divide a value from it.  

Comparison Operators: == (is equal to), != (is not equal to), <, >, >= (is greater than or equal to), <=.  These are used to compare two values and return a boolean result (true or false). These are often used in conjunction with: 

Logical and/or operators (and = &&, or = ||) to create more specific scenarios, such as if(a==b && b==c)

Modular Operator: % is used to calculate a remainder. This is useful because integers discard the remainder when divided.

Increment/decrement operators allow us to simply increase or decrease the value of a variable. 
	++a or a++; //adds 1 to the value of a
	--a or a--; //subtracts 1 to the value of a
If used as a prefix, it adds/subtracts 1 before any other operation the variable is being used for. As a postfix, the line of code it is embedded in runs before the variable is modified.

Ternary Operator is (condition) ? true : false. It is very similar to an if/else statement, but can sometimes be a more efficient way of accomplishing the same thing.
<>


[3.6] Loops (8:53)
------------------
Think of a scenario while using a mobile app that might require you to use a
"continue" statement in the middle of a loop.

**ANSWER HERE**<>In any case where you're searching an array for items which meet a condition and then modifying those items, you would want to skip any item that did not match your criteria, without ending the search.<>

[3.7] Functions (10:16)
-----------------------
What is a function? What is a function prototype? What are the purposes of each?
What are the rules for when and how you can call a function?

**ANSWER HERE**<>A function is a section of code wrapped up and given a name, so that it can be called by other functions. A function prototype exists to give the compiler a heads-up that a given function is going to exist later in the code. 

In both the function header and prototype, the format is:
returnType functionName (requiredArguments)

Without a prototype, a function can only be called after its code has been defined in the project. With or without a prototype, a function must be given any input parameters it requires to function.<>


Section 4: Variables
====================
[4.1] Data types (7:06)
-----------------------
What are the primitive data types in Objective-C? Why did Apple add a set of
classes to handle other data types?

**ANSWER HERE**<>int, float, double, char, and bool.
int = integer from -2.147 to 2.147 billion.
float = floating point number (a number with decimal point data)
double = also a floating point number, but twice as large
char = a character
BOOL = YES or NO
Apple provided classes to handle other data types (which are just combinations of the primitive ones) to make things easier on us! Otherwise, we'd have to re-write the code for handling strings each time we wanted to use them. <>

[4.2] Working with numbers (9:33)
---------------------------------
Make a table of Objective-C primitive data types. Add numeric data types and
their properties to this table.

**PRETTY TABLE GOES HERE**<>
|Data Type|Bytes|Properties|
|int||4 bytes|-2,147,483,648 to 2,147,483,647|
|float|4 bytes|will render as a double unless you end the value with f|
|double|8 bytes|contains decimal data.|
|unsigned int|4 bytes|0 to 4,294,967,295|
|long int|32-bit: 4 bytes 64-bit: 8 bytes| -9223372036854775808 to 9223372036854775807|
|long long int|8 bytes|-9223372036854775808 to 9223372036854775807|
|short int|2 bytes|-32767 to 32768|
|char|1 byte|one ascii character|
|bool|1 byte|YES or NO|

[4.3] Working with characters (4:39)
------------------------------------
Add char and BOOL (the character data types) to your table created above.

**ANSWER ABOVE!**

[4.4] Variable scope (8:06)
---------------------------
Describe in your own words what the scope of a variable is in Objective-C

**ANSWER HERE**<>A local variable in Objective-C only exists within the boundaries of the statement block that defined it, or other nested statements within that block. The only way to make a global variable is to define it outside of any function. This allows you to re-use variable names (even though that's still not the best idea for clarity's sake).<>



[4.5] Enumerations (3:35)
-------------------------
What does the `enum` keyword allow you to do?

**ANSWER HERE**<>It allows you to define a variable with a much more limited set of possible values, stored internally as integers. For instance, 

enum puppy {basenji, schnorkie};

creates a variable called puppy that has only two possible values, basenji or schnorkie.<>

[4.6] Using typedef (2:17)
--------------------------
When would you define your own data type versus using an enum?

**ANSWER HERE**<>It makes it slightly simpler to create new instances of that data type, because you can just type

puppy louis = basenji;

instead of 

enum puppy louis = basenji;

It's a pretty small change, but makes typing out lots of variables a little less clunky, and isn't too much more complex than defining the enum was in the first place.<>

[4.7] Preprocessor directives (5:56)
------------------------------------
Describe the three common preprocessor directives, `#import`, `#define`, and
`#if DEBUG`. Come up with one example where you would use each.

**ANSWER HERE**<>
 #import tells the compiler that your code may refer to things contained in whatever file we import. we pretty much always need to import foundation.h, because it contains things like NSString, BOOL, and dozens of pre-defined values.
 #define sets a permanent unchangable value to something. This is useful for reference numbers like e and pi, as well as any other numbers you want to access but not accidentally change.
 #if DEBUG allows you to write code which will only be included in the compiled result if you run the program in debug mode. This allows you to hide inner workings from end-users, but explicate what's going on in debug mode so that it's easier to track what's happening where in your code.
 
 <>
 

[4.8] Working with strings (7:52)
---------------------------------
Define the same string using both NSString and C-style string syntax. Describe
the purpose behind each part of your definition.

**ANSWER HERE**<>In most other C-style languages we can just write something like:
string puppy = "Arf, Arf!"; 

where string is the data type, puppy is the desired name of our string, and "Arf, Arf!" is the value.

but in Objective-C, we use NSString objects instead of a built-in String data-type, so it's a bit more complicated:

NSString *puppy = @"Arf, Arf!"; 

where NSString is the object type, * is a pointer to where the object will be stored, puppy is the name of the object, @ tells the compiler that this is a bit of Objective-C and not plain C, and "Arf, Arf!" remains the value of the string.

In both cases, ; tells the compiler that that line of code is complete.<>




Section 5: Classes
==================
[5.1] Introduction to object orientation (7:36)
-----------------------------------------------
Create an encapsulated (including generalized attributes and behavior)
description of a `MobileMakersParticipant` class. Instantiate a single object
representing yourself as a member of this class.

**DO YOU PROMISE YOU DID IT?**<>Yep!<>

[5.2] Using objects and pointers (6:38)
---------------------------------------
What is the pointer’s role in instantiating an object from a class? How is a
pointer different than a primitive?

**ANSWER HERE**<>We don't know how large an object is in the memory, so it's easier to point at it than it is to move around the full value of it.<>

[5.3] Messages and methods (6:44)
---------------------------------
What is the main difference between Objective-C’s messages and method calls in
other languages? How can this difference be seen as an advantage while
programming?

**ANSWER HERE**<>The main difference is the absence of dot syntax and the presence of square brackets.  While this creates some silly-long method names, the advantage is that the method call itself becomes very readable.<>

[5.4] Using existing classes in the foundation framework (8:40)
---------------------------------------------------------------
What's the difference between a class method and an instance method?

**ANSWER HERE**<>A class method is designed to work on the entire class, while an instance method is designed to work on an instance of the object. Many instance methods involve manipulating the data within the object, while class methods are often referential.<>

Try typing "NSD..." into your code window. Use the autofill feature and select a
single class name that starts with those three letters. Once the name has been
auto-completed, use the handy shortcut (Option + click) and investigate the
class whose name just got printed to the screen. Examine the task list for this
class. Do this a few more times until you're familiar with the process, or until
you've exhausted your curiosity, whichever comes last.


Section 6: Memory Management
============================
[6.1] What's new with memory management? (1:45)
-----------------------------------------------
Let it soak in. No questions for this one.

**PHEW**<>Thank god!<>

[6.2] Memory management in Objective-C (6:58)
---------------------------------------------
What is the relationship between a pointer to an object, a block of memory, and
the owning and releasing process. Can you come up with an analogy for this
relationship?

**ANSWER HERE**<>The pointer stores the location of the object, which is in a block of memory. If you own an object, you should release it when done with it. Otherwise, you should leave it alone.  This is similar to how the internet works. A URL serves as a pointer to where a website is stored. <>

[6.3] Object creation (7:31)
----------------------------
What does the new method do when used to create an object instance of a class?
Why do we avoid using this method? How long is an object's lifetime?

**ANSWER HERE**<>new will allocate a segment of memory for the object, initialize it (to zero/null for all values), and return the memory address as a pointer. It's not bad, per se, but many objects have an init method which will create the object instance with default values instead of null values. Objects live for the duration of the program, or until released.<>

[6.4] Using autorelease pools (5:14)
------------------------------------
How does the autorelease pool work? How and when can you use it deliberately?

**ANSWER HERE**<>While release means release now, autorelease means release later. Objects are released from the autorelease pool, typically at the end of the main function or at the end of every event loop. Autorelease is most useful when you are returning an object from a function.<>

[6.5] Apple autoreleased objects (3:39)
---------------------------------------
What does ARC stand for? Why is it important to remember this?

**ANSWER HERE**<>Automatic Reference Counting? But I think you might have meant NARC, which is New, Alloc, Retain, Copy, which are the keywords you need to look for to know what must be released.<>

[6.6] Introduction to Automatic Reference Counting (ARC) (4:43)
---------------------------------------------------------------
What does ARC save us from having to do? How does it keep us from having to make
this extra effort?

**ANSWER HERE**<>ARC uses the compiler to auto-fill the retain and release calls, so that we don't have to manage all of this manually.<>

[6.7] What ARC manages (2:42)
-----------------------------
What are the differences between ARC and garbage collection? What makes these
differences advantageous?

**ANSWER HERE**<>Garbage Collection occurs in real-time, requiring CPU power and occasionally slowing down programs. ARC occurs at compilation, doing the work for you before the program has ever run.<>

[6.8] The rules of ARC (4:20)
-----------------------------
Why can you not release or dealloc memory when working with ARC?

**ANSWER HERE**<>If you manually released or deallocated memory while working with ARC, it could interfere with the automatic count.<>


Section 7: Custom Classes
=========================
[7.1] Creating your own classes (14:01)
---------------------------------------
What are the two different sections used to create a class? What do they hold
and what files are they placed in?

**ANSWER HERE**<>the interface and implementation sections. the interface is made in a .h file, and is a rough outline, just explicating what the object will contain and what it will do.  the implementation then must actually contain/do everything promised by the interface file.<>
    
**Challenge!** Create a Tweet class for a twitter style app.
 
[7.2] Defining methods (8:36)
-----------------------------
**Challenge!** Define what should get passed in and what should get returned by
each of your methods in your Tweet class above.

**DO YOU LIKE TWITTER?**<>Not particularly. I think it has niche marketing and crowdsourcing uses, and is an interesting display of how small the world has become, but it's used far more often for annoying, insipid uses than for good ones.<>

[7.3] Defining properties (7:21)
--------------------------------
How did Objective-C programmers handle instance variables before 2012? How are
they handled now? What got easier and what got obscured?

**ANSWER HERE**<>Previously we defined them as regular variables in the interface .h file, and had to manually create methods to get and set the value for each of those variables. Now we use the @property signifier to automatically generate those accessor methods.<>

[7.4] Defining initializers (12:30)
-----------------------------------
What are initializers and why do we need to use them? Describe a situations when
you can rely on the standard `init` method and when you have to create your own
custom initializer.

**ANSWER HERE**<>Initializers ensure that objects are created with useful values. If we are creating an puppy object, for instance, the adorable BOOL should be set to YES for all new puppies. <>

[7.5] Using dealloc (5:33)
--------------------------
Why can we have a dealloc method in a class when using ARC, but we can't call
dealloc manually oursevles when using ARC?

**ANSWER HERE**<>The dealloc method what ARC calls to deallocate memory so writing a new one doesn't change that or mess with the ARC count, it merely modifies the behavior of the delloc method in question.<>


Section 8: Collections
======================
[8.1] Working with C-style arrays (7:12)
----------------------------------------
What are the three constraints when using C-style arrays? Create a C-style array
that holds the days of the week.

**ANSWER HERE**<>No Bounds Checking - you can attempt to access or fill part of the array that doesn't exist, fixed size - you cannot add or remove a slot to/from the array after creation, and can't mix types - an int array can only contain integers, an object array can only contain one type of objects. 
NSString *daysOfWeek[7] = {@"Sunday",@"Monday",@"Tuesday",@"Wednesday",@"Thursday",@"Friday",@"Saturday"};
<>

[8.2] Working with Objective-C array objects (8:00)
---------------------------------------------------
What is the difference between a mutable and an immutable array?

**ANSWER HERE**<>a NSArray object is immutable - cannot be changed after creation. NSMutableArray objects can be modified, added to, etc.<>

**Challenge!**<>
Create an immutable array containing the days of the week. Create a mutable
array that contains the days of the week that you will be at Mobile Makers. Add
the days of the week from the immutable array to the mutable array.
<>
NSArray *daysOfWeek = [NSArray arrayWithObjects:@"Sunday", @"Monday",@"Tuesday",@"Wednesday",@"Thursday",@"Friday",@"Saturday", nil];

NSMutableArray *daysAtMobileMakers = [NSMutableArray arrayWithObjects:@"Monday",@"Tuesday",@"Wednesday",@"Thursday", nil];

[daysAtMobileMakers addObjectsFromArray:*daysOfWeek];
<>

[8.3] Using dictionaries (5:55)
-------------------------------
Create a dictionary that lists five or more events in your life and the
accompanying year (or date if you want to get fancy) of the event.

**MAKE IT SO** <>
NSDictionary *events =
    [NSDictionary dictionaryWithObjectsAndKeys:
     @"Rode my bike across the USA", @"2003",
     @"Born", @"1985",
     @"Moved to Chicago", @"2005",
     @"Met Chris", @"2011",
     @"Purchased Condo", @"2012",
     @"Adopted Puppies", @"2013",
     nil];
    
    NSString *someYear = @"2013";
    
    NSLog(@"In %@ I %@.", someYear, [events objectForKey:Someyear]);
<>

[8.4] Fast enumeration (3:27)
-----------------------------
Use fast enumeration to log the timeline of the life events you described above
to the console.

**AYE AYE CAPTAIN**<> 

for (NSString *year in events){
	NSLog(@"In %@ I %@.", year, [events objectForKey:year]);
}
<>
Section 9: File Management
==========================
[9.1] Introduction to file management in Objective-C (6:44)
-----------------------------------------------------------
What can you do with files using the methods you are aware of that are available
in Objective C’s Foundation class?

**ANSWER HERE**<>NSFileManager allows us to copy, move, verify, delete, manage attributes of files. <>

[9.2] Working with paths and URLs (7:17)
----------------------------------------
What are the three parts of a URL? What are the advantages to using NSURL?

**ANSWER HERE**<> The scheme (HTTP://, FTP://, file://, etc), domain (www.mobilemakers.co, localhost, etc), and path(/ios-bootcamp/index.html). URLS are faster than path strings, better for catching erroes, and are used by more classes.<>

[9.3] Reading and writing strings (4:38)
----------------------------------------
What would be a reason you would want to write a string to disk instead of just
keeping it memory?

**ANSWER HERE**<>Data stored on the disk is far more permanent. If you expect a different program to want to look at data or a user to reboot their machine before you need to access it again, you will need to store it to disk. It also frees up memory for the rest of your program to use, if you're not going to need something for a while.<>

[9.4] Archiving objects (12:41)
-------------------------------
Why would you want to archive an object instead of writing the data to disk
using the techniques discussed previously?

**ANSWER HERE**<>Archiving comes with a simple methodology for unarchiving, which re-builds the object that we archived. Otherwise, we'd need to read the data back and make a new object with the same name as the original. They accomplish the same thing, but archiving is much more streamlined and comes built-in.<>


Section 10 - More Complex Classes
=================================
[10.1] Inheritance and NSObject (8:13)
--------------------------------------
How can you determine what methods you're inheriting from a super class? How do
you overide a method inherited from a super class?

**ANSWER HERE**<>To determine what we're inheriting, the most straightforward way is to look at the documentation for the superclass.

To override, we merely need to write a method with the same name in our subclass.<>

[10.2] Extending classes with categories (6:31)
-----------------------------------------------
What is the difference between a category and an inheritance? What are the
limitations of using a category?

**ANSWER HERE**<>Categories add new functionality to existing classes, without having to subclass and change any of your object types. You cannot, however, safely override original methods of the class you are making a new category on. You also cannot add new instance variables.<>

[10.3] Defining protocols (5:14)
--------------------------------
How are protocols useful?

**ANSWER HERE**<>Protocols provide a uniform way of interacting with different objects. Objects that wish to use any functionality provided by a protocol must adhere to its requirements, which often means writing specific methods that accomplish specific things.<>

[10.4] Dynamic typing (11:33)
-----------------------------
What are the advantages and disadvantages to dynamic typing?

**ANSWER HERE**<>Dynamic typing allows you to write code when you don't know yet what type of object is going to hold some data, and figure that out later. It's more likely to break if it looks for and doesn't find some functionality, but the compiler won't find the error.<>
