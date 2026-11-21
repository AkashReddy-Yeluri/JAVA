### JDK, JRE, JVM & JIT

These four terms are closely related and are among the most important fundamentals

You have written the code, but the computer cannot directly execute Java source code as native CPU instructions.

Java needs components that can:
- Compile Java source code.
- Load compiled classes.
- Execute Java bytecode.
- Provide built-in libraries.
- Optimize execution for better performance.
  
This is where JDK, JRE, JVM, and JIT come into the picture.

#### JVM (Java Virtual Machine)

It is the runtime engine responsible for executing Java bytecode.

The JVM is a virtual machine, an abstract computer that has its own ISA, memory, stack, heap, etc. It runs on the host OS and places its demands for resources on it

The JVM is a specification and can have different implementations, as long as they adhere to the specs

The operations defined inside the spec are:

* The 'class' file format
* Data types
* Primitive types and values
* Reference types and values
* Run-time data areas
* Frames
* Representation of objects
* Floating-point arithmetic
* Special methods
* Exceptions
* Instruction set summary
* Class libraries
* Public design, private implementation

#### JRE (Java Runtime Environment)

It provides the environment required to run Java applications. Conceptually, it includes the JVM along with the supporting libraries and runtime components needed to execute Java programs.

Think of it this way:

You have already written and compiled your Java program. Now you need an environment in which it can run.

The JRE provides that runtime environment.

What does the JRE contain?
- JVM — executes Java bytecode.
- Java class libraries — provides built-in functionality such as collections, strings, input/output, networking, etc.
- Other supporting runtime components.

Example:

Suppose you develop a banking application using Java that allows customers to check their balance, transfer money, and view transaction history.

You write and compile the code using the JDK. Once the application is ready, the customer doesn't need to write or compile any Java code. They only need to run the application.

The JRE basically provides the environment required to run the Java application, including the JVM and supporting libraries.

In simple terms:
- JDK – Used by developers to develop and compile Java programs.
- JRE – Provides the environment to run Java programs.

Some real-world examples of Java runtime environments are:
- Oracle Java Runtime
- OpenJDK Runtime
- Eclipse Temurin

#### JDK (Java Development Kit)

It is the package used by developers to develop, compile, debug and run Java applications.

If you want to write Java code, compile it, and execute it, you need a JDK.
What does the JDK contain?
- Java compiler (javac)
- JVM
- Runtime libraries
- Java development tools (such as javadoc, jar, debugging tools and other utilities)

we basically use command (java -version) in command prompt to find installed java version

#### JIT (Just-In-Time Compiler)

It is a component of the JVM that improves program execution performance by compiling frequently executed bytecode into native machine code at runtime.

Why do we need JIT?

Imagine your application has a method that calculates tax, and that method is called 10 lakh times.

The JVM may initially execute the method using its bytecode interpreter. While the program runs, the JVM identifies frequently executed code (often called hot code).

Instead of interpreting that code repeatedly, the JIT compiler can compile it into native machine code, which can execute more efficiently.



## Difference between JDK, JRE, JVM and JIT

| Component | Full form | Purpose |
|---|---|---|
| **JDK** | Java Development Kit | Develop, compile, debug and run Java programs |
| **JRE** | Java Runtime Environment | Provides runtime components to run Java applications |
| **JVM** | Java Virtual Machine | Loads and executes Java bytecode |
| **JIT** | Just-In-Time Compiler | Compiles frequently executed bytecode into native machine code to improve performance |