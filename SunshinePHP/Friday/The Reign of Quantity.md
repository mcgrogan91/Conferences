# The Reign Of Quantity, or Why Two are Better Than One
Matthew Meier O'Phinney

[@mwop](https://twitter.com/mwop)

[Joind link](https://joind.in/talk/97b67)

Project lead on Laminas project. Product Manager, Zend by Perforce

## What is Quality?

Requires an understanding of the system as a whole

Skill acquisition is a series of spikes and plateaus

How to we learn Quality?  We practice (with quantity)

### What do we practice?

#### Coding Standards
* Just use one! Just choose one and stick with it
* Integrate it into your editors
* Helps with consistency, readability

#### Testing and making testable systems
Things to think about:   
 
* Start to think about when tests are necessary.
 * One off scripts
 * Places where the language will ensure correctness (type hints, etc)
* Covering your paths
 * Ensure your tests cover all paths through a function
* Parameter overloading
 * Can often lead to untestable functionality, too many permutations
 * If a lot of args are to build something, tell them to build it themselves
 * You can create multiple methods with different parameters so it's clear what each is doing

#### S.O.L.I.D.
* Single Responsibility Principle
* Open-Closed Principle
* Liskov Substitution Principle
* Interface Segregation Principle
* Dependency Inversion Principle

#### Refactoring
* Extract Method
* Extract Class
* Extract and Generalize Types

#### Code Calisthenics
* Only One Level of Indentation Per Method
* Don't Use the ELSE Keyword
* Wrap All Primitives and Strings
* First Class Collections
* One Dot Per Line
* Don't Abbreviate
* Keep All Entities Small
* No Classes With More Than Two Instance Variables
* No Getters/Setters/Properties


These are just more rules.  You have to internalize them, through practice.

Ask for peer review.  Work with junior members of your team, where you explain things to them which helps learning for yourself.


