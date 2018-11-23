# Introduction to Spring WebFlux

**TL:DR:** An introduction to the article giving a brief summary of the what the article
will focus us.

## Prerequisites
Softwares you need to install to follow the tutorial:

* JDK 10
* Any text editor or IDE of your choice, though I recommend Intellij

## Theoretical Foundation for Spring WebFlux

### Problem Statement: Blocking I/O
* Briefly explain it.

### Solution: Non-Blocking Asynchronous I/O
* Briefly explain the solution.

### What is Reactive Programming?
* Introduce reactive programming as described by the reactive manifesto.

### What is Non-Blocking Programming?
* Non-Blocking I/O and its implications.
* Why has become important.

### What is Asynchronous Programming?
* Introduce Asynchronous programming.
* Why it matters?

### Benefits of Reactive programming

## Reactive Programming with Reactive Streams
* Introduce Project Reactor as an implementation of reactive streams.
* What are Reactive Streams and what is their specifications.

### Reactive Streams DataFlow
* Lifecycle of data in reative streams

### Project Reactor's implementation of Reactive Streams
* Reactor's data types for reactive streams.
* Reactor's operators for reactive streams.

## What is Spring WebFlux
* Introduction to Spring WebFlux.
* Discuss Key features of Spring WebFlux (Annotated Controllers, WebClient,
  Functional Endpoints).
* How is it different from Spring MVC.
* Spring WebFlux's promises.

## Developing a RESTful API with Spring WebFlux
* Setup MongoDB movie database.
* Create an entity for Movies.
* Create Movie Repository.
* Add initial data to the Movie database.
* Create a controller to query our database using the Annotated Controllers
fashion and Functional endpoints style.

## Securing your Spring WebFlux API with Auth0
* Add security configurations in `application.yml`
* Add a Security class to decode authentication tokens.

## Testing Your API
* Test the API with curl and a Auth0 access token.

## Conclusion
* Remind the reader what he/she learned in the article.
* Tell them what other things they could do with Spring WebFlux and point them
towards additional resources.
