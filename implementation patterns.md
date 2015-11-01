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


# Implementation Patterns
