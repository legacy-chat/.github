# LegacyChat
I know what all of you want: to be able to use Discord on a 20 year old PowerPC mac running MacOS 10.4 Tiger, but you can't because Electron doesn't support it for some reason. That's why I'm creating a full chat client in Java 5, the latest version officially supported by MacOS 10.4 Tiger.

## What we have
### Generics
Newly added for Java 5, generics allow better type saftey for certain design patterns. Hurray.

### The Collections Framework
Lists and Maps and other collection classes. Using the new generics included in Java 5.

### Annotations
Another new Java 5 feature: annotations contain informations about classes and methods that can be used at compile time or run time.

### Varargs
The last parameter of a function can be variadic allowing functions to accept an arbitrary number of arguments.

### java.util.concurrant
Also new for Java 5, Java provides a number of classes to make concurrent programming easier like futures and thread pools.

### Java Swing
A fine UI library, Java Swing "provides a set of 'lightweight' components that, to the maximum degree possible, work the same on all platforms." I am aware that Swing is "uncool" but if it runs J2SE 5 is probably supports Swing perfectly which fits with our goal of compatability.

### JUnit
The latest version of JUnit 4.13.2 works perfectly on Java 5. Thank you JUnit for still supporting Java 5, I'm sure we make up a very small percentage of your users and I become more and more aware as I write in Java 5 the sort of language features we are missing out on.

## What we need
### JSON
Google Gson is only avaliable for Java 6 and later. We will need to spin up something ourselves. A bit of an odd requirement we have is that we ought to be able to read JSON objects out of a stream to support Discord gateway.

We have some work going on a library at 
[legacy-json](https://github.com/legacy-chat/legacy-json)

### Logging
log4j also only supports Java 6 and up. As much as using older versions of some libraries couldn't hurt, I think we can all agree that using an outdated version of log4j is a particularly bad idea.

### Web sockets
We need an implementation of web sockets. These aren't very complicated and should go rather smoothly.

## What we don't have
### Diamond operator
Added in Java 7
### Binary integer literals
Added in Java 7
### Lambdas
Added in Java 8
### JEP 150: Date & Time API
Added in Java 8

