# Module 1 Notes
Notes for module 1 of CS121, Welcome to CS1. 

## 1.1 & 1.2 Programming
A **program** is a series of instructions executed by a computer.

The instructions are called **statements**. Each statement ends in a **semicolon**.

**Variable**: Variables hold varying values that are set by the user or another part of the program. A variable must be created before being assigned a value.

**Intput**: Input commonly comes from a keyboard, file, web form or app. The following code enables a program to get input `import java.util.Scanner;`

A **Scanner** is a text parser that can get numbers, words or phrases from an input source. Use `scnr.nextInt();` to get input from a keyboard.

**Output**: `System.out.print` supports output. Output is achieved with `System.out.print("desired text")`. Text in the double quotes is called a **string literal**

`System.out.println("")` prints and starts a new line.

To output multiple items use `+`: `System.out.print("sometext" + variable);`

## 1.3 & 1.4 Comments & Whitespace
**Comment**: Added by the programmer to help understand the code. Comments are ignored by the compiler.

**Single-line Comment**: starts with //. Includes anything on the line after //.

**Multi-line Comment (Block Comment)**: starts with /* and ends with */. all text between the symbols is part of the comment. 

**Whitespace**: Whitespace is blank space. It helps keep things readable. Companies and teams usually have set whitespace conventions.

- Use blank lines to separate conceptually distinct statements.
- Indent lines the same amount.
- Align items to reduce visual clutter.
- Use single space between operators like =,+,*, or / for readablility.
- End output with a new line.

## 1.5 Errors and Warnings
**Syntax error (Compile-time error)**: Incorrect syntax. A violation of the rules of the programming language (ex. forgetting the semicolon at end of statement).

**Run Time Errors**: Program compiles but when executed it terminates abnormally.

**Unclear error messages**: Error messages are often unclear or misleading. Look to previous lines to find real source of error.

**Logic errors (bugs)**: When a program compiles fine but has a flaw, this is called a logic error or bug.

**Compiler warnings**: Compiler still works but there is a possible logic error. Java can be run as `jvac -Xlint yourfile.java` to display all recommended warnings, otherwise we might miss some.

In general, when multiple errors are generated, start at the first one.

Compile and run frequently.

## 1.6 Computers and Programs
**Switches**: Allow or prohibit flow of electricity based on it's position. Engineers treat positive voltage as "1's" and zero voltage as "0's". These are known as **bits** (binary digits). **Circuits** are connections of switches.

**Processors**: processors execute a list of desired calculations, or **instructions**.

**Memory**: A circuit that can store bits at addressed locations.

### Writing computer programs
**High-level language**: Human readable, translated to machine instructions with a **compiler**. 

**Assembly language**: Human-readable processor instructions.

**Machine instructions**: 1's and 0's. Readable by the computer. This is what the computer runs in the background.

**Executable program**: a series of machine instructions. 

## 1.7 The Computer
**Input/output devices**: screen and keyboard, for example.

**Storage**: A disk that stores files and other data. Non-volatile, meaning it retains memory when powered off. Accesses memory in many clock ticks.

**Random Access Memory (RAM)**: temporary storage for data. Can be read and written much faster than a disk. Volatile, loses memory when powered off. Memory size typically in bytes (8 bits). Accesses memory in few clock ticks.

**Processor**: Runs calculations, or whole programs. When powered on, it runs the first set of instructions, usually a **basic input-output system (BIOS)**. The next set of instructions is usually the **operating system (OS)**. Usually contains small amount of RAM, called **cache**.

**Cache**: small amount of memory accessible very very quickly (one clock tick).

**Clock**: Instructions execute at a rate coverned by the processor clock. Frequency of clock ticks is measured in Hz, MHz, and GHz. Higher frequency is faster.

**Moore's Law**: the doubling of **IC** capacity every ~two years.

## 1.8 Language History

- 1978: Brian Kernighan & Dennis Ritchie of Bell Labs publish book on **C**, named after another language called B. C was dominant in 80's and 90's.
- 1985: Bjarne Sroustrupp publishes book describing **C++**. C++ is based on C with added constructs to support object-oriented programming. The ++ part refers to the ++ operator in C that increases a number.
- 1991: James Gosling begin developing JAVA language with the goal of creating a language whose exec. can be ported to different processors.
- 1995: Java is released.

Java was initially developed for appliances like TV's but then web browsers started to support it, increasing its popularity.
Java and JavaScript are entirely distinct.

## 1.9 Problem Solving
Just as a chef may write a new recipe in English, but must know more than just the English language, a programmer must know more than just a language, they must also know how to problem solve.

**Problem solving**: Creating a methodical solution to a task.

In this chapter we answered several problem solving questions and not much else. 

Key takeaway: programmers should come up with a solution before writing a program.

