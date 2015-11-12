# Values

* Communication

* Simplicity

* Flexibility


# Principles

* Local Consequences
Structure the code so changes have local consequences. If a change here can cause a problem there, then the cost of the change rises dramatically.

* Minimize Repetition
A principle that contributes to keeping consequences local is to minimize repeti- tion. When you have the same code in several places, if you change one copy of the code you have to decide whether or not to change all the other copies. Your change is no longer local. The more copies of the code, the more a change will cost.

* Logic and Data Together
Put logic and the data it operates on near each other, in the same method if possible, or the same object, or at least the same package. To make a change, the logic and data are likely to have to change at the same time. If they are together, then the consequences of changing them will remain local.

* Symmetry
An add() method is accompanied by a remove() method. A group of meth- ods all take the same parameters. All the fields in an object have the same lifetime. Identifying and clearly expressing symmetry makes code easier to read.
Symmetry in code is where the same idea is expressed the same way everywhere it appears in the code.

* Declarative Expression
express as much of my intention as possible declaratively. 

* Rate of Change
Put logic or data that changes at the same rate together and separate logic or data that changes at different rates.
All the fields in a single object should change at roughly the same rate.
The rate of change principle is an application of symmetry, but temporal symmetry. 


# Implementation Patterns

* Class
Each class is a declaration, “This logic goes together and changes more slowly than the data values on which it operates. These data values also go together, changing at similar rates and being operated on by related logic.”

Learning how to bundle logic in classes and express variations in that logic is part of programming effectively with objects.

Reducing the number of classes in a system is an improvement, as long as the remaining classes do not become bloated.

* Simple Superclass Name
Once classes have been named, the names of operations follow.
There is a tension between brevity and expressiveness. The names should be short and punchy. However, to make the names precise sometimes seems to require several words.
A way out of this dilemma is picking a strong metaphor for the computation. With a metaphor in mind, even single words bring with them a rich web of associations, connections, and implications. 
Look for one-word names for important classes.

* Qualified Subclass Name
The names of subclasses have two jobs. They need to communicate what class they are like and how they are different. 
Prepend one or more modifiers to the superclass name to form a subclass name.
One exception to this rule is when subclassing is used strictly as an implementation sharing mechanism and the subclass is an important concept in its own right.

Communication with people is the purpose of class names.
Use class names to tell the story of your code.


* Abstract Interface
Code to interfaces, not implementations.
A design decision should not be visible in more places than necessary.

Every layer of interface has costs. It is one more thing to learn, understand, document, debug, organize, browse, and name. Maximizing the number of interfaces doesn’t minimize the cost of software. Pay for interfaces only where you will need the flexibility they create.

Most software doesn’t need to be flexible in most of the ways it could be.

