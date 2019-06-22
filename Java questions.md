* OOPS Concept---
* How Abstraction Works
      Abstraction as an OOP concept in Java works by letting programmers create useful, 
      reusable tools. For example, a programmer can create several different types of objects. 
      These can be variables, functions, or data structures. Programmers can also create different classes of objects. 
      These are ways to define the objects.

      For instance, a class of variable might be an address. The class might specify that each address object 
      shall have a name, street, city, and zip code. The objects, in this case, might be employee addresses, 
      customer addresses, or supplier addresses.

* How Encapsulation Works
      Encapsulation lets us re-use functionality without jeopardizing security. It’s a powerful OOP concept in Java because 
      it helps us save a lot of time. For example, we may create a piece of code that calls specific data from a database. 
      It may be useful to reuse that code with other databases or processes. Encapsulation lets us do that while keeping our 
      original data private. It also lets us alter our original code without breaking it for others who have adopted it in the 
      meantime.

* How Inheritance Works
      Inheritance is another labor-saving Java OOP concept. It works by letting a new class adopt the properties of another. 
      We call the inheriting class a subclass or a child class. The original class is often called the parent. We use the 
      keyword extends to define a new class that inherits properties from an old class.

* How Polymorphism Works
      Polymorphism in Java works by using a reference to a parent class to affect an object in the child class. 
      We might create a class called “horse” by extending the “animal” class. That class might also implement the 
      “professional racing” class. The “horse” class is “polymorphic,” since it inherits attributes of both the “animal” and 
      “professional racing” class.
      Two more examples of polymorphism in Java are method overriding and method overloading.
      In method overriding, the child class can use the OOP polymorphism concept to override a method of its parent class. 
      That allows a programmer to use one method in different ways depending on whether it’s invoked by an object of the             parent class or an object of the child class.
      In method overloading, a single method may perform different functions depending on the context in which it’s called. 
      That is, a single method name might work in different ways depending on what arguments are passed to it.
      
      
      ================================================================================
      
  * Best Practices for OOP Concepts in Java
       Since the aim of OOP concepts in Java is to save time without sacrificing security and ease of use, the best practices        are all oriented toward advancing that main goal.

      DRY--- (Don’t Repeat Yourself). This is the core concept in Java. You should never have two blocks of identical code in       two different places. Instead, have one method you use for different applications.
      
      If you expect your Java code to change in the future, encapsulate it by making all variables and methods private at 
      the outset. As the code changes, increase access to “protected” as needed, but not too public.
      
      Single Responsibility. ----Another best practice for OOP concepts in Java is the Single Responsibility Principle. 
      Simply put, a class should always have only one functionality. That way, it can be called and/or extended on its own           when new uses arise for it, without causing coupling between different functionalities.
      
      Open Closed Design. ----Make all methods and classes Closed for modification but Open for an extension. That way, 
      tried and tested code can remain static but can be modified to perform new tasks as needed.
      
      =================================================================================
