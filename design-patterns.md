#Design patterns
Notes from design patterns books and trainings

- Identify the aspects of your application that vary and separate them from what stays the same
- Program to an interface, not an implementation
- Favor composition over inheritance
- Strive for loosely coupled designs between objects that interact
- Code should be closed to modification and open to extension
- Dependency inversion - dependency upon abstractions, not concrete classes
- Principle of Least Knowledge - talk only to your immediate friends
- The Hollywood principle - Don't call us, we'll call you
- Single responsibility - a class should have only one reason to change

##Strategy
Defines a family of algorithms, encapsulates each one, and makes them interchangeable.
Strategy lets the algorithm vary independently from clients that use it.

##Observer
Defines one-to-many dependency between objects so that when one object change state, all of its dependents are notified and updated automatically.

##Decorator
Attaches additional responsibilities to an object dynamically. Decorators provide a flexible alternative to subclassing for extending functionality.

##Factory method
Defines an interface for creating an object, but lets subclasses decide which class to instantiate.
Factory method lets a class defer instantiation to subclasses.

##Abstract factory
Provides an interface for creating families of related or dependent objects without specifying their concrete classes.

##Singleton
Ensures a class has only one instance, and provides a global point of access to it.

##Command
Encapsulates a request as an object, thereby letting you parametrize other objects with different requests, queue or log requests, and support undoable operations.

##Adapter
Converts the interface of a class into another interface the clients expect.
Adapter lets classes work together that couldn't otherwise because of incompatible interfaces.

##Facade
Provides a unified interface to a set of interfaces in a subsystem. Facade defines a higher level interface that makes the subsystem easier to use.

##The template method
Defines the skeleton of an algorithm in a method, deferring some steps to subclasses.
Template method lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure.

##Iterator
Provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation.

##Composite
Allows you to compose objects into tree structures to represent part-whole hierarchies.
Composite lets clients treat individual objects and compositions of objects uniformly.

##The state pattern
Allows an object to alter its behavior when its internal state change. The object will appear to change its class.

##Proxy
Provides a surrogate or placeholder for another object to control access to it.