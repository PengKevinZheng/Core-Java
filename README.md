# Core-Java

OOP

OOP properties: 

1. encapsulation

Encapsulation is the technique of making the fields in a class private and providing access to the fields via public methods. 

If a field is declared private, it cannot be accessed by anyone outside the class, thereby hiding the fields within the class.

Modifier    | Class | Package | Subclass | World



public      |    y    |     y    |      y     |     y



protected   |     y    |      y    |      y     |     n



no modifier |     y    |      y    |      n     |     n    **also known as package-private**



private     |     y    |      n    |      n     |     n



2. inheritance

Java Inheritance defines an is-a relationship between a superclass and its subclasses. This means that an object of a subclass can be used wherever an object of the superclass can be used. Class Inheritance in java mechanism is used to build new classes from existing classes. The inheritance relationship is transitive: if class x extends class y, then a class z, which extends class x, will also inherit from class y. 


3. polymorohism

a. overload:

Method Overloading is a feature that allows a class to have two or more methods having same name.

Argument lists could differ in

    1. Number of parameters.
 
    2. Data type of parameters.

    3. Sequence of Data type of parameters.

Notes: If two methods has same name, while they have difference parameters, then their retrun type does not matter at all.

If two methods has same name, while they have same parameters, there will be compling error.

Rules for Method Overloading:

Overloading can take place in the same class or in its sub-class.

Constructor in Java can be overloaded

Overloaded methods must have a different argument list.

Overloaded method should always be the part of the same class (can also take place in sub class), with same name but different parameters.

The parameters may differ in their type or number, or in both.

They may have the same or different return types.

It is also known as compile time polymorphism.

b.override:

Rules for Method Overriding:

applies only to inherited methods

object type (NOT reference variable type) determines which overridden method will be used at runtime

Overriding method can have different return type (refer this)

Overriding method must not have more restrictive access modifier

Abstract methods must be overridden

Static and final methods cannot be overridden

Constructors cannot be overridden

It is also known as Runtime polymorphism.




 


4. abstraction 
5. 
1) Use abstraction if you know something needs to be in class but implementation of that varies. Abstraction is actually result of thought process and it really need good experience of both domain and Object oriented analysis and design to come up with good abstraction for your project.

2) In Java you can not create instance of abstract class using new operator, its compiler error. Though abstract class can have constructor.

3) abstract is a keyword in Java, which can be used with both class and method.  Abstract class can contain both abstract and concrete method. Abstract method doesn't have body, just declaration.

4) A class automatically becomes abstract class when any of its method declared as abstract.

5) abstract method doesn't have method body.

6) In Java, variable can not be made abstract , its only class or methods which would be abstract.

7) If a class extends an abstract class or interface it has to provide implementation to all its abstract method to be a concrete class. alternatively this class can also be abstract.

Difference between abstract class and Interface:

Abstract class 	        Interface 
Partial implementation 	No implementation 
Single inheritance 	    Multiple inheritance 
ANY methods 	        [public abstract] methods (default to be) 
ANYfileds 	            [public static final] fields (default to be) 
Better performance 	    Lazy-loading 






