# Core Java
* JVM -> Virtual machine where the code runs.
* JDK -> Provides tools for Development(Compilers ...)
* JRE -> Provides JVM and other lib for the code to run

Object -> Representation of states and behavior of real world Objects
Class  -> Blueprint on which Objects are created

# OOPS 
* Inheritance
  State and Behaviour inherited from super classes
  * Contract between class and outside world
  * Hiding details and showing functionality
  Example -
* Encapsulation
  Hiding Internal Details -> Achieved using getters and Setters
  Example -
* Abstraction 
  Hiding implementation -> Achieved using abstract and Interfaces
  Example -
* Polymorphism
  Object having different forms
  * Subclasses define its own behaviour , but same functionality of the Parent class
  * Interface/Parent class type
  Example -
    
## Inheritance
  * Get the state and Behaviour from the super classes
  * Object class is the super class for all classes
  * Multiple Inheritance not allowed
      * Two classes having a method with a same signature

  1. Static methods with same signature in child class - Method hiding
  2. Instance methods with same signature in child class - Method over-riding
  3. Methods with same name anbd different parameters - Method overloading
  4.  Inherited instance methods from classes can override abstract interface methods

#### Overloading methods
* Different Parameters(By type or by Numbers)
* The compiler does not consider return type when differentiating methods
* In method overloading , the most specific version is choosed  for the type
  When overloading a method , the Access level cannot be reduced
#### Overriding methods
Method return Type - You can reurn an object which is of same type , or a Subclass of it

## Polymorphism
   * Subclasses define its own behaviour , but same functionality of the Parent class
    
# Data Type
byte - 8 bit
short - 16 bit
int - 32 bit
long - 64 bit
float - 32 bit
double - 64 bit
char -16 bit

Uninitialized local variable -> Compile time error
Prefix 0x->Hexa 0b->Binary

# Variables 
* Class Variables (Static variables)
* Instance Variables
* Local Variables 

# Constructors
- Called when the object is created
- Default constuctor is implicitly called
- The subclass constructor implicitly calls the default constructor of the Parent
  - It is always better to have a Default constructor along with the Parametrized constructor ,
    as it does not mandate the subclass to call the parametrized constructor.

# Access Modifiers
* Public
* Private - Restricted to own class
* Protected - Restricted to the sublclasses
* Default - Restricted to packages

Access Levels

Modifier	 | Class	| Package	| Subclass | World |
| -------- |:------:| -------:|---------:|------:|
public	 | Y	| Y	| Y	 | Y     |
protected	 | Y	| Y	| Y	 | N     |
no modifier| Y	| Y	| N	 | N     |
private	 | Y	| N	| N	 | N     |

# Final Modifier
  - Variable - it`s value cannot change
  - Method - Cannot be overridden by the sub-classes
  - Class - Cannot be sub-classed

# Static - Common across instances
  - A static method cannot access this keyword ,as the Keyword belongs to instance

# Creating Objects
  - new
  - Class.forName().newInstance()
  - clone() - Should implement Clonable Interface
  - Deserialization - Reading from File

# Object class methods
  - clone - Class should implement Clonable Interface
  - equals
  - finalize , called by Garbage collector to garbage collect
  - getClass
  - hashCode
  - wait , Causes the current thread to wait until another thread invokes the notify() method or the notifyAll() method for this object.
  - Notify all - Wakes up a single thread that is waiting on this object's monitor.

# Initialization 
## Static field
- Using static block
## Instance field
- Using final methods or initializer blocks

# Interface
- Provides contract between class and the real world
- All the methods dont have implementation
- All the methods are public by default
- Interface can be used as a Type
- Use default and static methods - To extend the Interfaces
  - Class extending two Interfaces having same signature Default methods , Compile time Error

System.arrayCopy
Arrays -> copyOf
       -> binarySearch
       -> Sort
       -> Fill

Pre-Increment
Post-Increment

# Operator
* && , || exhibit short circuiting Behaviour
* ?: -> if-then-else
* null -> not instance of anything
* Switch case works for Numbers , Enums , Strings
* labeled, unlabelled break/continue

## Equals vs ==
== Works on Primitives only, checks if the references match
equals compares the actual Objects

# String, String Buffer and String Builder
* Strings
  * create using new keyword - >
  * toString
  * doubleQuotes
* String methods
  * charAt
  * length
  * concat
  * format
  * valueOf
  * equalsIgnoreCase
  * split
  * contains
  * startsWith
  * matches
  * indexOf
  * toUppercase
  * toLowercase
  * subString
  * trim
  * replace - accepts char
  * replaceAll - accepts regex and replacement string
* StringBuilder -mutable
 * capacity - default 16
 * append
 * insert
 * replace
 * delete
 * reverse
 
* StringBuffer - thraedsafe
* StringBuilder - not thread safe
* Autoboxing - Conversion of primitive to Wrapper type
* Unboxing - Conversion of Wrapper to primitive

# Java Pass by Value
  - When method is called , the Object reference is passed as value.
Call by value - The caller and calee has different varialbes
Call by reference - The caller and the calee has same variables

# Nested Classes
- Static- Static nested class
- non Static - Inner class
  * Anonymous - no name specified
  * Local - defined within a block
   * Cannot have static variables , as it belongs to instance of the Outer class
   * Can access variables that are declared final/ Effectively Final (Java8)
To access a variable outside scope of the Inner class(if the var is of same name) , use OuterClass.this.var

# ENUM - Set of predefined Constants
# Annotations
- Compiletime/Deployment time - @Override
- Runtime - JAXRS
- syntax @interface annotationname{}
@Retention - When that annotation is used
@Target - Where can the annotaion be applied

# Character class
- isDigit
- isLetter
- isUpperCase
- isLowerCase
    
# Immutable - Cannot change
- final class type
- no setters

# String pools(partition in Heap)
-> Strings are most used components , hence Strings are stored in String pool for 
re-usablity
-> String literals are re-used(loaded from pool) if the same String literal is used again.
-> Strings created using new keyword gets created in Heap even if the value is present in pool 

# Generics - More detectible bug during compile time
- Strong compile time checks
- Write generic algorithm
- Elimination of Casts

Generic classes are defined by class name followed by Type variable
Raw Type - When a generic class is instantiated without type
Generic Methods - define their own type parameters , parameters defined just before the return types
Lower bound Wildcards - to work with any class and its superclasses - super keyword
Upper bound Wildcards - to work with any class and its subclasses - extends keyword
Type Erasure - Java compiler replaces the Type parameters with corresponding Bounds

# Exception - An event which distrupts the actual flow of the Program
Exception propogates from the place where exception occurs through the stack trace till it finds an exception handler
Throwable ->Error & Exception
Types
- Checked Exceptions
- Error
- Runtime Exceptions
If a catch block handles more than one exception type, then the catch parameter is implicitly final.

# I/O Stream - input source or an output destination
Input/Output Stream - R/W Bytes
Readers/Writers - R/W Characters
Scanner , Printer - Human readable form
Files , Paths - File operations

# Process , Threads
* Process - Program execution
* Thread  - Part of Process

Thread - Path followed when executing a Program
Multithreading - Two or more tasks getting executed concurrently
-Implementing Runnable
-Extending Thread

Thread.sleep - > throws InterruptedException

Interrupt -> Stop the continuous process
Thread.interrupted () -> to check if thread is Interrupted
T.interrupt() -> to Interrupt a thread
T.join -> stops the current thread till the Execution of T is completed

* When one thread is executing a synchronized method for an object, all other threads that invoke synchronized methods for the same object block (suspend execution) until the first thread is done with the object.

* When a thread invokes a synchronized method, it automatically acquires the intrinsic lock for that method's object and releases it when the method returns

wait -> thread to wait notifyAll -> wake up from wait

# JDBC
- Create a Connection
- Craete a Statement
- Execute a Query
- Process resultset
- Close connection

- Statement.addTOBatch
- Statement.executeBatch
- ResultSet.moveToCurrent/InsertRow
- statement.executeUpdate
## Transaction
A transaction is a set of one or more statements that is executed as a unit,
so either all of the statements are executed, or none of the statements is executed.
### Transaction Levels
- None
- Read Uncomitted
- Reads comitted
- Repeatable-Read
- Serializable

### Savepoint - Multiple transactions
- conn.setSavepoint()
- conn.rollBack(svpt)
- conn.releaseSavePoint(svpt)
System and env variable
Null values in collection

# JPA - ORM Framework
Object Relational Framework
Entity - A class persisted in a database
@Transient - Field not to be saved in Database
Entity Manager - manages the entities and propogates the change to the database


persist - entity becomes managed
detach - entity not managed
      - done to edit the entity offline , then attached using merge operation
managed - entity attached to persistance context
@Embeddable - Componenet to be embeded
Composite primary key
  @EmbededID
@Temporal is used to map java.sql.XXX to java.util.XXX
bidirectional
@ManytoOne - JoinColumn
@OneTomany - mapped by , maintain relationship

Inheritance (@Inheritance , Strategy =)
  - Single table - @Disctiminator column to describe the Descriminator, @DiscriminatorValue to describe the values in the SubClasses
  - Joined Table - @PrimarykeyJoinColumn
  - Table per class
  - Mapped super class

Difference between Joined Table and Table per class ,
  In Table per class , The subclasses will have all the columns present in the parent class1

Query
  - Entitymanager.createQuery
  - Entitymanager.createNamedQuery

# J2EE
## Servlet Interface
- init
- destroy
- service
- getServletInfo
- getServletConfig

### HTTPServlet
- doGet
- doPost
- doXXX

### LifeCyle of Servlet
* Servlet class is loaded.
* Servlet instance is created.
* init method is invoked.
* service method is invoked.
* destroy method is invoked.

Web container calls all the init,destroy,service methods

  web.xml
    - servlet (servlet name , servlet class)
    - servlet mapping (servlet name , url pattern)
  Session Tracking
    Cookies - setMaxAge , getName ,getValue
    Hidden Form Field
    URL Rewriting
    HttpSession

  RequestDispatcher.include -> to forward requests
      session.getAttribute("xxx");  -> to get data from session
      session.invalidate(); -> to invalidate a session
  Filter
    - init
    - destroy
    - doFilter
  Filter (filter-name , filter-class)
  Filter mapping (filter-name,filter-url)
  <servlet>
    <load-on-startup>
      -> If greater than Zero , it starts the servlets(call init method) in that order

  Session Tracking is a way to maintain state of an user.

# REST - An architecture style for networking application
* Resource identification through URI
* Manuplate the resource using database

# Webservices
- Based on WSDl
- Use XML , and SOAP protocol
- Advantages - Uses WS-*** Protocols for Security, QoS
  @WebService , @WebMethod(operation)

# WSDL
* Types– a container for data type definitions using some type system (such as XSD).
* Message– an abstract, typed definition of the data being communicated.
* Port Type–an abstract set of operations supported by one or more endpoints.
* Binding– a concrete protocol and data format specification for a particular port type.
* Port– a single endpoint defined as a combination of a binding and a network address.
* Service– a collection of related endpoints.

# Patterns
Singleton -> creates single Instance
Facade  -> hides the sub-system implementation to the clients ,and acts as single point of contact
Factory -> Object creation -> Subclasses responsible for Object creation
Adaptor -> mapping from one interface to another interface

# Spring
  - Light weight Java Framework - Alternative to EJB
  Modules
          - core
          - mvc
          - testing
          - aop
          - data-access
          - security
   Features
          - IOC - Inversion of control
                    - Objects dont create the objects , containers create them
                 Dependency Injection
                    - Provides dependencies during run-time
   Predifined templates for JDBc, JPA , Hibernate
   Loosely coupled , because of Dependency injection
   
   Bean Factory
          - Used to create Beans , Provides basic functionality
   Application Context
          - Provides functionality to Enterprise applications
   
   Container(AppliactionContext) is responsible for creation of beans , assembling and configuring them.
   
   XML Based Configuration
   Annotaion Based Configuration
   Java Configuration
   
   A bean is an object that is instantiated, assembled, and otherwise managed by a Spring IoC container
   
   A CONTAINER provides an execution environment that is responsible for adding the technical concerns to the COMPONENTS
   
   The id should be unique for a Bean. A bean can have multiple names .If an id is not given to a bean , the container will generate its own id 
