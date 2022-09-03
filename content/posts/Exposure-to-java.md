---
title: "Exposure to Java"
date: 2022-09-02T07:52:16+05:30
draft: false
---

# Java 

 - Java is class-based and object-oriented.
 - It is platform-independent
    - java code can be compiled on any operating system and made to run on the same or any other operating system.
 - It supports concurrency
    - which means multiple processes can execute the code at the same time. Many java programming statements can be executed together instead of executing in one by one in sequence.

## Features

  - Portability: java source code can be developed and compiled on one machine and can be made to run on the same or any other operating system.
  
  - Object-Oriented: Everything is treated as an object, and all the operations involved in application development are completed using these objects.
  
  - Dynamic Capability: Applications developed using java can adapt them to changing execution environment. This is because this programming language has features like dynamic memory allocation in which the amount of memory allocated changes according to the environment, which in turn provides high performance.
  
  - High Security: Java operates on byte code which is not readable in nature. It runs source code inside a secured sandbox and does not allow any external intervention.
  
  - Robust:  It allows developing code that handles all possible errors. Also, it has a strong type checking that makes our source code robust.
  
  - Multithreading: It supports creating multiple threads for execution, thus providing high performance. Also, it supports the synchronization mechanism to maintain synchronization between different threads.
  
  - Interpreted: The code is converted into byte code, which is interpreted by the java run time environment.
  
  - Distributed: It supports developing distributed applications. It provides features like Remote Method Invocation, through which a program can communicate with another program present in the remote machines through the network and generates the desired output.
  
  - Performance: It provides high performance as it uses bytecode, which can be translated into machine code with ease and high speed. It has Just in time compiler through which high performance is achieved.

## Code execution

```sh
$ javac HelloWorld.java
$ java HelloWorld
```

### Variable declaration

```java
int i = 10;
String name = 'John';
float num = 2.2;
char a = 'A';
```

### Recursion

```java
class Factorial {
  public static void main(String[] args) {
    System.out.println(factorial(0));
    System.out.println(factorial(3));
    System.out.println(factorial(5));
  }

  public static int factorial(int number) {
    if(number == 0)
      return 1;

    return number * factorial(number - 1);
  }
}
```
```java
class Fibonacci {
  public static int nthFibonacci(int term) {
    if(term == 1)
      return 0;
    if(term == 2)
      return 1;

    return nthFibonacci(term - 1) + nthFibonacci(term - 2);
  }

  public static void printNthFibonacci(int term) {
    System.out.println(term + "th term fibonacci : " + nthFibonacci(term));
  }

  public static void main(String[] args) {
    printNthFibonacci(5);
    printNthFibonacci(7);
    printNthFibonacci(6);
    printNthFibonacci(5);
    printNthFibonacci(4);
    printNthFibonacci(3);
    printNthFibonacci(2);
  }
}
```