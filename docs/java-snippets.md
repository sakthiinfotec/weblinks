#### Java Code Snippets

[Inject values into a Map from the properties file using the @Value annotation](https://stackoverflow.com/a/51997862/337011):

```java
@Value("#{${user}}")  
private Map<String, String> user;
```

Entry in application.properties must be:

```sh
user = { "name" : "John", "age" : "35", "place" : "California" }
```

### Functional Interface

![image](https://github.com/user-attachments/assets/a8e5d248-5ca2-4d37-9fe6-4f65aa6162de)

In Java, a functional interface is an interface that contains exactly one abstract method, allowing it to be used with lambda expressions and method references.  
Here's a more detailed explanation:

• Single Abstract Method (SAM): The defining characteristic of a functional interface is that it must have only one abstract method.
• Lambda Expressions and Method References: Functional interfaces are designed to be used with lambda expressions and method references, providing a concise way to implement the single abstract method.
• Example: 
```java
    @FunctionalInterface
    interface MyFunctionalInterface {
        void doSomething();
    }
```
In this example, MyFunctionalInterface is a functional interface because it has only one abstract method, `doSomething()`.

• `@FunctionalInterface` Annotation: While not mandatory, it's good practice to annotate an interface with `@FunctionalInterface` to indicate that it is intended to be a functional interface. This helps the compiler catch errors if the interface accidentally has more than one abstract method.
• Benefits:
	• Conciseness: Lambda expressions make code more concise and readable when implementing functional interfaces.
	• Flexibility: Functional interfaces enable functional programming techniques, such as passing behavior as parameters.
	• Readability: Lambda expressions directly represent the logic for the single method of the functional interface, making the code's intention clearer.

• Built-in Functional Interfaces: Java provides several built-in functional interfaces in the `java.util.function` package, such as `Consumer, Supplier, Function`, and `Predicate`.
