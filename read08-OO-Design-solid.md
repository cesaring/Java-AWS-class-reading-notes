**SOLID**

**S** Single-Responsibility Use principle --

All classes should have a single responsibility. Mostly this means that things like printing output should be handled by handling classes.  The functions in a class should 
worry about handling state.

**O** open for extensibility, closed for modification.

With good design, adding features would be available for classes by extending an existing class, and not by modifying an existing class

**L** Lipskiv(?) principle.

Child classes should be able to stand in for parent classes.  Don't try to methods to class that it's children will not need/use/irrelevant.

**I** Interface Segregation Principle
The interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface. in short, you don't want to force clients to depend on things they don't actually need. 


**D** Dependency Injection
When possible, create abstract(?) classes that can handle a variety of specific subclasses, without the need to write subclass specific code in the consuming class.

