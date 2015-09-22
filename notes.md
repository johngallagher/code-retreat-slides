# Intro

Introduce yourself
Get the others to introduce themselves (name, role, experience with TDD)
I appreciate we have some testers with us today. Let's hear your background. Have you done any coding before?
Are you interested in learning about TDD?
We can do something about SpecFlow over lunch if you like?

Today we are taking part in a learning format called a CodeRetreat.
Today is a heavily practical focused training course on building confidence using techniques associated with TDD.
We will be split up in sessions, during which I will add a new learning point during each session.
Each session builds on the last. 

Not here to make progress. We are here to practice the craft of making programs.

Format: 45m coding, 10m review, 5m break
Oh and one more thing!

Qs before we start?

# Session 1

I'm going to want you to work in pairs or threes for the first session. No other constraints, no need to TDD anything.
Over today you'll be able to pair with everybody. As we will rotate pairs at the end of each session.
Get to know the problem
Same problem all day.

Conway's game of life. Cellular autama game. That mimics some simple rules for deciding who lives on and who dies.
4 Rules. Don't worry, i'll have them written up
Less than 2 dies
2 or 3 survices
4 or more dies
dead with 3 becomes alive

Qs

What approaches are people taking to the problem?
How are you feeling about deleting the code?

# Session 2

TDD

Technique to create code at a sustainable pace over the course of a project.
It involves writing an example of the code you wished you had first. 
Part of this example asserts that some condition has been met. Like the result of adding two numbers is 2.
Which won't even compile at first.
Make it compile, see the test runner bar turn Red
then meet the expectation in a test until it is Green
Once it is Green you have two choices. Add another failing test, or refactor the code.
Refactor means change the existing code to improve it's design or performances without adding any new featuers.
We'll have another session on refactoring later.  For this session we'll focus on the TDD aspect.

PingPong

A way of making sure a pair take turns creating production and test code.
production code is what you ship, test code does not ship, it is for providing a regresssion test suite for your code
I use this everyday for programming.

Qs

Ping pong TDD
TDD
What data structure are you prefering for resprensenting the cells?

# Session 3

Refactoring. Simple rules of design, renamed to Extreme Normal Form.
It's a list of conditions to meet in order to progress.
Inherit code from another pair.

Qs

How did you find following the rules?
How about inheriting someone elses code?

# LUNCH

# Cucumber

Business conversations about requirements. With the biz, tester and developer. Called a 3 amigos

Feature: Serve coffee
    In order to deliver a financially sound and responsible coffee experience
    As a responsible vending machine operator
    I want Coffee to not be served until paid for
    I want the customers money to be refunded if there is no coffee left

  Scenario: Buy last coffee
    Given there are 1 coffees left in the machine
    And I have deposited 1$
    When I press the coffee button
    Then I should be served a coffee

VS can autogenerate the matching rules
End to end tests
A few end to end tests
Or make the tests run under the UI, so they are fast and not brittle
Who writes the code? Anyone who can write production code. If they cannot write production code they must pair until they can.

# Session 4

Mute Evil Programmer
You can write on paper to share what you mean, but I'd encourage you to find a way to communicate via the code.
Wrtie great test names, great variable, method, class and package names. Clearly show your intent.

Evil person. Make the laziest solution to what the tests  force you to, until it is easier to just implement the solution they want you to do.

Qs

How was being quiet?
Fake it until you make it is a real approach


# Session 5

Objected Orientated Principles

No Booleans.
Primitive Obsession

Booleans: Often can be replaced with Objectes. WE can end up with two classes in one with a bunch of behavuour the changes based on that state.
Prime use of inheritence. Live Cell and Dead Cell
Polymorphism is better than booleans

Primitive Obsession: We tend to write a bunch of primitives like ints, floats, Strings and keep them together. Instead we should extract them into objects.
Those objects will become attractive, and should pull in behaviour that was elsewhere.

The Smell: Primitive Obsession is using primitive data types to represent domain ideas. 
For example, we use a String to represent a message, an Integer to represent an amount of money, or a Struct/Dictionary/Hash to represent a specific object.
Example magic: Date formatting. All parsing and formatting ends up with the valueobject.

Qs

How was this constraint?
Did anyone try anything to avoid primitive obsession?

# Session 6

Pick two constraints

Qs

What, if anything, did you learn today?
What, if anything, surprised you today?
What, if anything, will you do differently in the future?

