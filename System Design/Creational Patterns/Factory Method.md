


**Factory method** is a creational design pattern which solves the problem of creating product objects without specifying their concrete classes.

That is, when there is a superclass and multiple subclasses, and we want to get object of subclasses based on input requirements. Then we create factory class which takes the responsibility of creating object of subclasses based on input and requirement.


The Factory Method defines a method, which should be used for creating objects instead of using a direct constructor call (`new` operator). Subclasses can override this method to change the class of objects that will be created.




<img src="https://refactoring.guru/images/patterns/diagrams/factory-method/structure.png">
