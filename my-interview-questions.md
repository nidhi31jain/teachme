* What Is Spring or Spring Framwork?<br>
Spring is a development framework. 
The core features of the Spring Framework can be used in developing any Java application, but there are extensions for building web applications. <br>
Spring framework targets to make development easier to use and promote good programming practice.<br>
Spring framework created to address the complexity of enterprise application development<br>

* What Are Benefits Of Using Spring<br>
  * Inversion of control (IOC): Loose coupling is achieved in spring using the technique Inversion of Control. 
  The objects give their dependencies instead of creating or looking for dependent objects.
  * Aspect oriented (AOP): Spring supports Aspect oriented programming and enables cohesive development by separating application business logic from system services.
  * Container: Spring contains and manages the life cycle and configuration of application objects.
  * MVC Framework: Spring's web framework is a well-designed web MVC framework, which provides a great alternative to web frameworks such as Struts or other over engineered or less popular web frameworks.
  * Transaction Management: Spring provides a consistent transaction management interface that can scale down to a local transaction (using a single database, for example) and scale up to global transactions (using JTA, for example).
  * Exception Handling: Spring provides a convenient API to translate technology-specific exceptions (thrown by JDBC, Hibernate, or JDO, for example) into consistent, unchecked exceptions.

* What Are The Different Modules In Spring Framework
  * Core module
  * Bean module
  * Context module
  * Expression Language module
  * JDBC module
  * ORM module
  * OXM module
  * Java Messaging Service(JMS) module
  * Transaction module
  * Web module
  * Web-Servlet module
  * Web-Struts module
  * Web-Portlet module
  
* What Is Dependency Injection? (Need to Remember the defination)<br>
  Inversion of Control (IoC) is a general concept, and it can be expressed in many different ways and Dependency Injection is merely one concrete example of Inversion of Control.This concept says that you do not create your objects but describe how they should be created. You don't directly connect your components and services together in code but describe which services are needed by which components in a configuration file. A container (the IOC container) is then responsible for hooking it all up.
  
* What Are The Types Of Dependency Injection Spring Supports
  * Setter Injection: Setter-based DI is realized by calling setter methods on your beans after invoking a no-argument constructor or no-argument static factory method to instantiate your bean.
  * Constructor Injection: Constructor-based DI is realized by invoking a constructor with a number of arguments, each representing a collaborator.
  
* What Is Aop?<br>
  Aspect-oriented programming, or AOP, is a programming technique that allows programmers to modularize crosscutting concerns, or behavior that cuts across the typical divisions of responsibility, such as logging and transaction management. The core construct of AOP is the aspect, which encapsulates behaviors affecting multiple classes into reusable modules.
  
* What Bean(Object we create through @Bean annotation) Scopes Does Spring Support? Explain Them.?<br>
  The Spring Framework supports following five scopes, three of which are available only if you use a web-aware ApplicationContext.
  * singleton: This scopes the bean definition to a single instance per Spring IoC container.
  * prototype: This scopes a single bean definition to have any number of object instances.
  * request: This scopes a bean definition to an HTTP request. Only valid in the context of a web-aware Spring ApplicationContext.
  * session: This scopes a bean definition to an HTTP session. Only valid in the context of a web-aware Spring ApplicationContext.
  * global-session: This scopes a bean definition to a global HTTP session. Only valid in the context of a web-aware Spring ApplicationContext.
  
* What Is Default Scope Of Bean(Object we create through @Bean annotation) In Spring Framework?<br>
  The default scope of bean is Singleton for Spring framework.

* Are Singleton Beans(Object we create through @Bean annotation) Thread Safe In Spring Framework?<br>
  No, singleton beans are not thread-safe in Spring framework.
  
* What Does @qualifier Annotation Mean?<br>
  There may be a situation when you create more than one bean of the same type and want to wire only one of them with a property, in such case you can use @Qualifier annotation along with @Autowired to remove the confusion by specifying which exact bean will be wired.</br>
  Example : you have to call two database oracle and my sql , so you need two JdbcTemplate for two databases
  ```javascript
  @Bean
  @qualifier("oracle")
  JdbcTemplate getOracleJdbcTemplate(){...}
  ```
  ```javascript
  @Bean
  @qualifier("mysql")
  JdbcTemplate getMySqlJdbcTemplate(){...}
  ```
* What Is Spring Web Mvc Framework?<br>
  The Spring Web MVC framework provides model-view-controller architecture.<br>
  * M - Model - Pojo's, Object with setter getters
  * V - View - Html/JSP - User interface/UI/Any digital channels 
  * C - Controller - Rest Endpoints/ Rest Mappings based on path<br>
  Provide ready components that can be used to develop flexible and loosely coupled web applications.
  The MVC pattern results in separating the different aspects of the application (input logic, business logic, and UI logic), while providing a loose coupling between these elements.
  
* What Is Bean Factory?
A BeanFactory is like a factory class that contains a collection of beans. The BeanFactory holds Bean Definitions of multiple beans within itself and then instantiates the bean whenever asked for by clients.
* BeanFactory is able to create associations between collaborating objects as they are instantiated. This removes the burden of configuration from bean itself and the beans client.
* BeanFactory also takes part in the life cycle of a bean, making calls to custom initialization and destruction methods

* What Is Spring Boot?
First of all Spring Boot is not a framework, it is a way to ease to create stand-alone application with minimal or zero configurations. It is approach to develop spring based application with very less configuration. It provides defaults for code and annotation configuration to quick start new spring projects within no time. Spring Boot automatically configures required classes depending on the libraries on its classpath. Suppose your application want to interact with DB, if there are Spring Data libraries on class path then it automatically sets up connection to DB along with the Data Source class.

* What Are The Advantages Of Using Spring Boot?
It is very easy to develop Spring Based applications with Java or Groovy.<br>
It reduces lots of development time and increases productivity.<br>
It avoids writing lots of boilerplate Code, Annotations and XML Configuration.<br>
It is very easy to integrate Spring Boot Application with its Spring Ecosystem like Spring JDBC, Spring ORM, Spring Data, Spring Security etc.<br>
It follows “Opinionated Defaults Configuration” Approach to reduce Developer effort<br>
It provides Embedded HTTP servers like Tomcat, Jetty etc. to develop and test our web applications very easily.<br>
It provides CLI (Command Line Interface) tool to develop and test Spring Boot (Java or Groovy) Applications from command prompt very easily and quickly.<br>
It provides lots of plugins to develop and test Spring Boot Applications very easily using Build Tools like Maven and Gradle<br>
It provides lots of plugins to work with embedded and in-memory Databases very easily.<br>

* What Embedded Containers Does Spring Boot Support?
Spring Boot includes support for embedded Tomcat, Jetty, and Undertow servers. By default the embedded server will listen for HTTP requests on port 8080.

* What Is Actuator In Spring Boot?
Spring Boot Actuator is a sub-project of Spring Boot. It adds several production grade services to your application with little effort on your part. There are also has many features added to your application out-of-the-box for managing the service in a production (or other) environment. They’re mainly used to expose different types of information about the running application – health, metrics, info, dump, env etc.






  
