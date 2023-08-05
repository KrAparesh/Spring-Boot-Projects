# This is the beginning of a journey

I'll dive deep into the details of entities and keywords used while the writing the code. Before starting, here's a short summary of what we're trying to achieve. We'll be building a simple application that has the capability of performing CRUD operations.

[Spring Initializer](https://start.spring.io/)


# Foundation Structure

## @Controller

Upon application startup, a Spring Bean (object managed by Spring IoC container within the app) is created. It uses _View Resolvers_ to render HTML templates.

## @RestController

A combination of **@Controller** and **@ResponseBody**. It is primarily used for building APIs that return data in formats such as JSON, XML or other representation (JSON by default). 

## @RequestMapping

It maps HTTP requests to specific methods in a controller. (Here it's "coffees")

These annotations perform similar task:
* @GetMapping
* @PostMapping
* @PutMapping
* @PatchMapping
* @DeleteMapping

# More Datatypes in Java

## Optional<> 

`Optional` is a class introduced in Java 8 as part of the `java.util` package. It is used to represent an object that may or may not contain a non-null value. The primary purpose of `Optional` is to avoid `NullPointerExceptions` by explicitly indicating that a value may be absent.

In the context of Spring, methods can return `Optional` as a way to indicate that the result of the operation may or may not have a meaningful value. Instead of returning `null`, the method returns an `Optional` object, which allows the caller to explicitly check whether a value exists and handle the absence of a value gracefully.

Using `Optional` return types can encourage better practices when dealing with possibly null values and help make code more explicit about the presence or absence of a value.

## Iterable<>

 `Iterable` is a standard Java interface that represents a collection of elements and allows you to iterate over those elements. It's part of the `java.lang` package, and it is implemented by various classes like `List`, `Set`, and others.

In the context of Spring, methods returning `Iterable` are often used to represent collections of elements. For example, in the case of database queries, a method might return a list of objects representing the result set.

By using `Iterable` as the return type, the caller can iterate over the elements to process or display the collection.

##

*Conclusion* : `Optional` is used when returning a single result that may or may not exist, while `Iterable` is used for returning collections of elements that can be iterated over.
