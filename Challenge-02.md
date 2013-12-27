From the Lynda.com video series “Foundations of Programming: Object-Oriented
Design”, watch each (short) video and answer the correlating questions:


Section 0: Introduction
=======================
[0.1] What to expect from this course (3:06)
--------------------------------------------
What is the intended purpose and potential advantage of learning object oriented
design?

**ANSWER HERE**<>The intended purpose is to write programs faster, with less bugs and more flexibility, by lessening our reliance on the code editor and spending more time thinking and storyboarding before writing code.<>

[0.2] Exploring object-oriented analysis, design, and development (1:41)
------------------------------------------------------------------------
Why might it be advantageous to analyze and design before beginning programming?

**ANSWER HERE**<>By explicating our intended outcome and methods, we organize our thoughts before starting to code, which ensures that everything is as organized as possible.<>

[0.3] Reviewing software development methodologies (4:08)
---------------------------------------------------------
What is the difference between a "waterfall" and an "agile" approach to
development? What is an iteration and how do we to use them to build software?

**ANSWER HERE**<>A waterfall approach is a strict linear plan with several steps, completing each step before beginning the next. An agile approach is more responsive to new ideas mid-implementation.  Each iteration contains its own analysis, design, and programming cycle. We expect the initial iteration to be incomplete and flawed, and each subsequent iteration to build on its predecessor.<>


Section 1: Core Concepts
========================
[1.1] Why we use object-orientation (2:42)
------------------------------------------
What are the various types of programming languages and in which domain is each
used?

**ANSWER HERE**<>Procedural languages are generally used for writing one long piece of code, and seem to be more or less obsolete as mainframes are replaced by more advanced, multi-tasking computers. Functional and Logic programming languages serve extremely niche uses in academia and linguistics. 
Object Oriented Languages - pretty much all of the popular languages made in the last two decades - contain self-contained objects with their own data and logic, which makes them much more modular and less dependent upon a complete plan being in place from the beginning.<>

[1.2] What is an object? (5:22)
-------------------------------
Describe in your own words the three properties of a computing object.

**ANSWER HERE**<>Identity: each object - even two iterations of the same object - is independent and unique.
Attributes: each object has a number of possible attributes based on its complexity, which describe their current state.
Behavior: things the object can do - functions that accomplish something.<>

[1.3] What is a class? (4:43)
-----------------------------
Explain how classes are analogous to blueprints. Include the relationship
between a class and an object. Can you think of how the analogy breaks down?

**ANSWER HERE**<>A class is like a blueprint in that it describes what the object will be and what its attributes will be.  The analogy breaks down a bit when it comes to classes also describing an object's behavior, as houses have decidedly few functions. It also breaks down in that an actual blueprint contains far more specific numbers when it comes to the dimensions of a house, whereas a house-object written as a class would merely mention that houses /have/ dimensions, not what they are.<>

[1.4] What is abstraction? (2:45)
---------------------------------
When a developer uses the term “abstraction” what are they describing?

**ANSWER HERE**<>An abstraction is a general idea that encompasses multitides of specific instances by focusing on the essential concepts and discarding unimportant details.<>

[1.5] What is encapsulation? (3:45)
-----------------------------------
What does encapsulation prevent? What does it enable?

**ANSWER HERE**<>Encapsulation protects objects by preventing outside tampering. It also enables us to change the way a class/object works without breaking the rest of our application.<>

[1.6] What is inheritance? (3:35)
---------------------------------
Describe the inheritance relationship between classes. When would this
relationship be advantageous to establish?

**ANSWER HERE**<>An inherited class is a new class based on an iteration of a previous class. The new class will automatically have every attribute and behavior of the old class, as well as any new attributes or behaviors we want to add. This is beneficial when we want to make an object similar to another we already have defined, but don't want to bog down the parent class with new data or functionality.<>

[1.7] What is polymorphism? (3:22)
----------------------------------
What is the basic idea behind polymorphism? How can it make the classes we
create more flexible?

**ANSWER HERE**<>The basic idea is to automatically perform the correct behavior depending on the situation or input. The most simple example here is that we can override inherited functions when that would be more useful than merely duplicating the functionality of the superclass. <>


Section 2: Object-Oriented Analysis and Design
==============================================
[2.1] Understanding the object-oriented analysis and design processes (4:13)
----------------------------------------------------------------------------
What are the steps of analysis that come before writing code for an application?
Why do you think these steps make writing the code easier?

**ANSWER HERE**<>Gather your requirements, Describe the App, Identify the main objects, describe the interactions, and create a class diagram. These effectively function as an outline or storyboard for the application we are trying to create, which gives us a fantastic starting-point for coding and keeps us organized.

[2.2] Defining requirements (6:09)
----------------------------------
What should you have after you've completed the first phase of defining your
requirements?

**ANSWER HERE**<>A list of all critical features and capabilities of the app. FURPS stands for Functional, Usability, Reliability, Performance, and Supportability, which can all have their own requirements. As can Design, Implementation, Interface, and Physical. The first iteration of this list should only contain what is absolutely necessary. <>

[2.3] Introduction to the Unified Modeling Language (UML) (1:54)
----------------------------------------------------------------
What is UML? Why Is it useful to visualize your application before coding it?

**ANSWER HERE**<>UML - the unified modeling language - is set of simple ways of diagramming pieces of code to assist us in the outlining/storyboarding process.<>

Section 3: Utilizing Use Cases
==============================
[3.1] Understanding use cases (6:11)
------------------------------------
Write a use case for creating an event on your phone's calendar.

**ANSWER HERE**<>Title: Create Calendar Event
Actor: User 
Scenario: 1) User taps "+" button on Calendar App
2) User inputs event details such as Name, Location, Time, and Date.
3) User is given opportunity to automate things such as reminder(s), invitations, and repeat events.
4) User taps "done" and Event is added to Calendar<>

[3.2] Identifying the actors (4:16)
-----------------------------------
Can you think of a use case for a mobile application in which the actor is not
the user of the mobile device?

**ANSWER HERE**<>If, say, an application is pulling pricing data from Amazon, the Amazon Server would be an Actor in that use case, responding to requests for data initiated by our user.<>

[3.3] Identifying the scenarios (5:07)
--------------------------------------
Write another use case for a mobile device user interacting with a calendar
application. This time include a couple extensions when crafting your scenario.

**ANSWER HERE**<>Title: Create Calendar Event
Actor: User, Invitee, System
Scenario: 1) User inputs event details
2) User confirms and Event is added to Calendar

Extensions: User invites others to her event; all invitees are added to "maybe" list.
	a) Invitee accepts; user receives an email confirmation and invitee is moved to "attending" list.
	b) Invitee declines; user receives an email confirmation and invitee is moved to "not attending" list.

Extensions: User repeats event
	a) One or more additional iterations of the event are added to the calendar.
	
Extensions: User requests notification when the event nears
	a) System notifies User in the manner requested.<>


[3.4] Diagramming use cases (4:18)
----------------------------------
Do a google image search for "use case diagram." Notice how many variations
there are. What do they all generally have in common?

**ANSWER HERE**<>They're all extremely easy to draw and to read, with minimalist elements like ovals, rectangles, stick-figures, and 1-3 word labels.<>

[3.5] Employing user stories (3:43)
-----------------------------------
Write 5 user stories to describe a mobile user interacting with his or her maps
application.

**ANSWER HERE**<>1)As a mobile user, I want directions to the nearest bike path, so that I can ride more safely.
2) As a mobile user, I want ETA of CTA buses and trains, so that I know when to leave my house.
3) As a mobile user, I want traffic data, so that I know which route to take.
4) As a mobile user, I want to know where I am, so that I don't get lost.
5) As a mobile user, I want to be able to easily measure distances, so that I know how far I am away from my destination.<>


Section 4: Domain Modeling (Modeling the App)
=============================================
[4.1] Creating a conceptual model (1:59)
----------------------------------------
What’s your favorite color?

**ANSWER HERE**<>Blue. No, Yellow!<>

[4.2] Identifying the classes (2:27)
------------------------------------
Identify the classes in the use case you constructed for a user interacting with
his or her calendar application in chapter 3.

**ANSWER HERE**<>User, Event, Calendar<>

[4.3] Identifying class relationships (2:38)
--------------------------------------------
Identify the relationships among the classes you found above. Create a
conceptual model where you diagram these relationships and then upload a picture
of your model below.

**ANSWER HERE**<>classrelationships2.4.3.PNG<>

[4.4] Identifying class responsibilities (6:43)
-----------------------------------------------
Identify the responsibilities of the classes you found above. List them here.

**ANSWER HERE**<>Create New Event, Add or Modify Event Details, Add Event to Calendar, Invite Invitees, Remind User, Repeat Event.

User: Invite Invitees (Invitees are users too!), Remind User
Event: Create New Event, Add or Modify Event Details, Repeat Event
Calendar: Add Event to Calendar<>

[4.5] Using CRC cards (2:49)
----------------------------
If you’d like, try creating CRC cards for the model you made above. There's no
need to respond here, just try it out and see if you like this form of
organization.

**ANSWER HERE… IF YOU LIKE** <>I like this better because you can rearrange them on the fly!<>


Section 5: Creating Classes
===========================
[5.1] Creating class diagrams (6:11)
------------------------------------
Construct Class Diagrams for the classes you imagine exist in a twitter app, a
maps app, a calendar app, or any other app you would like to make. Do you find
that it is easier to come up with the attributes or with the behaviors? Why do
you think that is?

**ANSWER HERE**<>Twitter App:
Class Name: User
Attributes: String: userName
	 int tweetCount
	 boolean privateMessages
	 icon 
	 background 
	 array following
Operations: modifyProfile() array 
	follow(user) boolean

Class Name: Tweet
Attributes: string tweet
	array hashtags
	boolean at
Operations: sendTweet() string
reTweet(user) string
search(string) array<>

[5.2] Converting class diagrams to code (4:57)
----------------------------------------------
How might the separation of interface and implementation in Objective-C be an
advantage when working with class diagrams?

**ANSWER HERE**<>the interface is fairly similar to a whole-picture diagram, caring only about what classes exist and how they interact. the implementation is more similar to an individual class diagram, and does the back-end work to make the relatively simple to read/write interface code function. Much like using instantiation and inheritance to reduce required code changes if we update/change something, this minimizes the amount of code we have to constantly rework/debug when we make a change.<>

[5.3] Exploring object lifetime (5:55)
--------------------------------------
What are the constructors and destructors in Objective-C? Why do we use them?

**ANSWER HERE**<> Constructor: init
Destructor:
We use constructors to initiate objects with useful properties instead of null/0 values for all of the variables. Destructors are automatically called when an object is deleted, and are used for releasing resources being used by the object before it is destroyed.<>

[5.4] Using static or shared members (5:22)
-------------------------------------------
Like the interest rate example in the video, give three additional examples of
data that would be the same for all instances of a class.

**ANSWER HERE**<> For all Clock Objects, the length of a day is 24 hours. For Taxi Rides, the fare meter formula is the same, depending on location/company. For any form of online or in-store shopping, Sales Tax is shared among all purchases.<>



Section 6: Inheritance and Composition
======================================
6.1 Identifying inheritance situations (6:49)
---------------------------------------------
Describe in your own words what inheritance is and how it is useful when
constructing classes.

**ANSWER HERE**<>it's much like the rectangle/square relationship, where squares share all of the qualities of a rectangle, as well as their own unique properties. 

it is tremendously useful and time-saving because it allows us to minimize duplicate code when multiple objects behave in similar ways.  it also allows us to modify or fix code in the parent class and have that proliferate down automatically to all subclasses.<>

[6.2] Using inheritance (2:43)
------------------------------
Referring to the apps on your phone, come up with three examples where you
believe methods are being inherited from superclasses and called by subclasses.

**ANSWER HERE**<>In my mobile banking apps, the checking and savings account are both likely subclasses of bankaccounts. In the Camera app, the new iOS7 camera filters are likely subclasses of the unfiltered camera results. The Music, Spotify, Podcast, and Pandora apps likely contain subclasses of the same audio playback API superclass.
