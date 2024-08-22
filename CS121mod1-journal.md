# Module 1 Notes
Notes for module 1 of CS121, Welcome to CS1. 

## Intro to Java
### Programs
A **program** is a series of instructions executed by a computer.

The instructions are called **statements**. Each statement ends in a **semicolon**.

### Variable
Variables hold varying values that are set by the user or another part of the program. A variable must be created before being assigned a value.

### Intput
Input commonly comes from a keyboard, file, web form or app. The following code enables a program to get input `import java.util.Scanner;`

A **Scanner** is a text parser that can get numbers, words or phrases from an input source. Use `scnr.nextInt();` to get input from a keyboard.

### Output
`System.out.print` supports output. Output is achieved with `System.out.print("desired text")`. Text in the double quotes is called a **string literal**

`System.out.println("")` prints and starts a new line.

To output multiple items use `+`: `System.out.print("sometext" + variable);`

### Comments
Comments are added by the programmer to help understand the code. Comments are ignored by the compiler.

**Single-line Comment**: starts with //. Includes anything on the line after //.

**Multi-line Comment (Block Comment)**: starts with /* and ends with */. all text between the symbols is part of the comment. 

### Whitespace
Whitespace is blank space. It helps keep things readable. Companies and teams usually have set whitespace conventions.

- Use blank lines to separate conceptually distinct statements.
- Indent lines the same amount.
- Align items to reduce visual clutter.
- Use single space between operators like =,+,*, or / for readablility.
- End output with a new line.

### Errors and Warnings
**Syntax error (Compile-time error)**: A violation of the rules of the programming language (ex. forgetting the semicolon at end of statement).

**Unclear error messages**: Error messages are often unclear or misleading. Look to previous lines to find real source of error.

**Logic errors (bugs)**: When a program compiles fine but has a flaw, this is called a logic error or bug.

**Compiler warnings**: Compiler still works but there is a possible logic error. Java can be run as `jvac -Xlint yourfile.java` to display all recommended warnings, otherwise we might miss some.

In general, when multiple errors are generated, start at the first one.

Compile and run frequently.

### Computers and Programs
**Switches**: Allow or prohibit flow of electricity based on it's position. Engineers treat positive voltage as "1's" and zero voltage as "0's". These are known as **bits** (binary digits). **Circuits** are connections of switches.

**Processors**: processors execute a list of desired calculations, or **instructions**.

**Memory**: A circuit that can store bits at addressed locations.

### Writing computer programs
**High-level language**: Human readable, translated to machine instructions with a **compiler**. 

**Assembly language**: Human-readable processor instructions.

**Machine instructions**: 1's and 0's. Readable by the computer. This is what the computer runs in the background.

**Executable program**: a series of machine instructions. 

### The Computer
**Input/output devices**: screen and keyboard, for example.

**Storage**: A disk that stores files and other data.

**Random Access Memory (RAM)**: 
