# Interview with ChatGPT - Java Core

## [Java] Can you give me some Java fundamental coding interview questions?

Sure! Here are some fundamental Java coding interview questions:

```dos
What is the difference between a class and an object in Java?
What is a constructor in Java, and how is it different from a method?
What is the difference between the "==" operator and the ".equals()" method in Java?
What is inheritance in Java, and how is it implemented?
What is encapsulation in Java, and why is it important?
What is polymorphism in Java, and how is it implemented?
What is a static method in Java, and how is it different from an instance method?
What is a final variable in Java, and how is it different from a constant?
What is a try-catch block in Java, and how does it work?
What is a thread in Java, and how can you create and manage them?
```

## [Java] What is a constructor in Java, and how is it different from a method?

In Java, a constructor is a special method that is used to create an object of a class. It has the same name as the class, and it is called when an object is instantiated. The purpose of a constructor is to initialize the instance variables of an object to their default values or to values specified by the programmer.

Here is an example of a constructor in Java:

```java
public class Person {
   private String name;
   private int age;

   public Person(String name, int age) {
      this.name = name;
      this.age = age;
   }
}
```

In this example, we have a constructor for the Person class that takes two parameters, name and age. The this keyword is used to refer to the instance variables of the Person object being created.

The main difference between a constructor and a method in Java is that a constructor has no return type, not even void, and it is always called when an object is created. On the other hand, a method has a return type and is called when the method is invoked. Additionally, a constructor is used to create objects, while a method is used to perform some action on an object or to return a value.

## [Java] What is the difference between the "==" operator and the ".equals()" method in Java?

In Java, the == operator is used to compare two objects to see if they are the same object in memory. On the other hand, the .equals() method is used to compare the contents of two objects to see if they are equal.

Here is an example to illustrate the difference:

```java
String a = "hello";
String b = "hello";
String c = new String("hello");

System.out.println(a == b); // true
System.out.println(a == c); // false
System.out.println(a.equals(b)); // true
System.out.println(a.equals(c)); // true
```

In this example, we have three string objects: a, b, and c. The first two objects are created using string literals, while the third object is created using the new keyword.

The first comparison (a == b) returns true because a and b are pointing to the same object in memory. The second comparison (a == c) returns false because a and c are two different objects in memory.

The third comparison (a.equals(b)) and the fourth comparison (a.equals(c)) both return true because the contents of the objects a, b, and c are all the same.

In summary, the == operator checks if two objects are the same object in memory, while the .equals() method checks if two objects have the same content.

## [Java] 2

## [Java] 3

## [Java] 21

## [Java] 31
