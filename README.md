## Java Language
---

### Releases, Versions and Features
[Java Versions and Features](https://www.marcobehler.com/guides/a-guide-to-java-versions-and-features)
[Java Version Features History](https://howtodoinjava.com/java-version-wise-features-history)
[JDK Release Notes](https://www.oracle.com/technetwork/java/javase/jdk-relnotes-index-2162236.html)

![Image](https://github.com/TheHun89/OOP/blob/master/images/oop.png)
![Image](https://media.geeksforgeeks.org/wp-content/uploads/java-collection.jpg)

Object – instance of a class that has identity, state and behavior, Object is the root class of all classes in Java

1.	Declaration: The code set in bold are all variable declarations that associate a variable name with an object type.
2.	Instantiation: The new keyword is a Java operator that creates the object.
3.	Initialization: The new operator is followed by a call to a constructor, which initializes the new object.
      Point originOne = new Point(23, 94);


[Memory](https://www.baeldung.com/java-stack-heap)

1.	Stack Memory
* Used for static memory allocation and the execution of a thread
* Contains primitive values specific to method and references to objects in heap
* When a new method is called, a new block on top of the stack is created which contains values specific to that method
* Access faster than heap and threadsafe
* StackOverFlowError – memory is full

2.	Heap Space
* Used for dynamic memory allocation for Java objects and runtime classes
* New objects are always created in heap space and references stored in stack
* OutOfMemoryError – heap space is full
* Slower, memory isn’t automatically deallocated, not threadsafe

![Image](memoryAllocation)


### Garbage Collection
Some object-oriented languages require that you keep track of all the objects you create and that you explicitly destroy them when they are no longer needed. Managing memory explicitly is tedious and error-prone. The Java platform allows you to create as many objects as you want (limited, of course, by what your system can handle), and you don't have to worry about destroying them. The Java runtime environment deletes objects when it determines that they are no longer being used. This process is called garbage collection.  An object is eligible for garbage collection when there are no more references to that object. References that are held in a variable are usually dropped when the variable goes out of scope. Or, you can explicitly drop an object reference by setting the variable to the special value null.
