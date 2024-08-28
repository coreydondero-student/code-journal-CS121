# Module 2 Notes
Notes for module 2 of CS121, Data and Expressions

## 2.1 & 2.2 Variables and Assignments
**Variable**: Named item used to hold a value.  
**Assignment**: Assigns a variable with a value. The left side is a variable and the right side is an expression.  
**Example**: x = 1, y = 2, x = y *2, x = x * 2  
**Variable Declarations**: A statement that declares a new variable. Ex: `int userAge;` declares a new integer type variable called userAge. The compiler allocates a memory location for userAge capable of storing an integer.  
**Allocation**: is the process of determining a suitable memory location to store data like variables.  
**Assignment Statement**: assigns the variable on the left-side of the = with the current value of the right-side expression. Ex: `numApples = 8;` assigns numApples with the value 8.  
**Expression**: A number like 8 or a calculation like `1 + numApples`  
**Integer Literal**: A number that appears in an expression, like 8 or 1.  
**Initializing Variables**: Sometimes an initial value is assigned when declared. Ex: `int numCars = 5`  

## 2.3 Identifiers  
**Identifier**: Name, given by the programmer, of a variable or method. 
 - Sequence of letters
 - Underscores
 - Dollar signs
 - Digits
 - Case sensetive
 - Start with letter, underscore or dollar sign, but _ and $ should be avoided in identifiers.
 - Can't be a reserved word.

**Identifier Styles**  
 - Camel Case, Lower Camel Case
 - Underscore seperated
 - Minimize abbreviations.
 - Meaningful name that describes items purpose
 - but not too long.

## 2.4 & 2.5 Arithmetic Expressions
**Expression**: any individual item or combination of items, like variables, literals, operators, and parentheses, that evaluates to a value, like `2 * (x + 1)`.  
**Literal**: a specific value in code like 2.  
**Operator**: a symbol that performs a built-in calculation, like +.  
**Evaluate**: Expressions evaluate to a value, which replaces the expression. Order of operation is followed: (), -, */%, +-, left to right.  
**Good Practice**: Use parentheses to be explicit even when it's not necessary due to order of operations. Helps find bugs.  
**Good Practice**: Single space around operators, except **unary minus** (negative sign).  
**Compound operators**: provide a shorthand way to update a variable, such as `userAge += 1` being shorthand for `userAge = userAge + 1`. Other compound operators include -=, *=, /=, and %=.  

## 2.7 Floating Point
**Floating-point number**: is a real number containing a decimal point that can appear anywhere (or "float") in the number. Ex: 98.6, 0.0001, or -55.667.  
**Double** variable stores a floating-point number. Ex: `double milesTravel;`  
**Floating-point literal**: is a number with a fractional part, even if the fraction is 0, as in 1.0, 0.0, or 99.573.  
**Warning** Best not to use floating point for money.  
**Division by zero**: error in most languages. In java it's infinity or -infinity. If numerator and denominator are 0, NaN (not a number).  
**Manipulating floating point**: To set the number of digits after the decimal to 2: `System.out.printf("%.2f", myFloat);`  

## 2.9 Constant Variables  
**Final**: prepend variable with `final` to fix the value. If the program tries to reassign the variable an error is produced. Ex: `final double SPEED_OF_SOUND   = 761.207;`.  
**Constant Variable**: An initialized variable whose value cannot change. Aka **final variable**. A common convention, or good practice, is to name constant variables using upper case letters with words separated by underscores, to make constant variables clearly visible in code.  

## 2.10 Integer Division and modulo  
 - With integer division answers are always rounded to whole numbers.
 - If at least one floating point is included, floating point division is used and so decimals are used.
 - For integer division, the second operand of / or % must never be 0, because division by 0 is mathematically undefined.
 - A **divide-by-zero** error occurs at runtime if a divisor is 0, causing a program to terminate. A divide-by-zero error is an example of a **runtime error**, a severe error that occurs at runtime and causes a program to terminate early.
**Modulo (%)**: evaluates the remainder of the division of two integer operands. Ex: 23 % 10 is 3.

## 2.11 Type Conversions  
A calculation will sometimes mix double and integer types. A **Type Conversion** is necessary. One type is converted to another.  
An **Implicit Conversion** is an automatic conversion that the compiler makes for common conversions like int -> double.  
 - For an arithmetic operator like + or *, if either operand is a double, the other is automatically converted to double, and then a floating-point operation is performed.  
 - For assignments, the right side type is converted to the left side type if the conversion is possible without loss of precision.
 - int-to-double conversion is straightforward: 25 becomes 25.0.  
 - double-to-int conversion may lose precision, so is not automatic.  
**Type Cast**: explicitly convert one data type to another.  Ex: If myIntVar is 7, then `(double)myIntVar` converts int 7 to double 7.0.

## 2.12 Binary  
**Binary Number**: Base 2, stored as 1's and 0's.  
**Decimal Number**: Base 10, stored as 0-9.  
**Example**: The compiler would convert the decimal number 212 to the binary number 11010100, meaning 1*128 + 1*64 + 0*32 + 1*16 + 0*8 + 1*4 + 0*2 + 0*1 = 212, and then store that binary number in memory.  

## 2.13 Characters  
Java does not have a method for getting one character from input. Instead, the following sequence can be used: `myChar = scnr.next().charAt(0);`  
Characters are stored internally as numbers. The compiler translates for you.  

## 2.14 Strings  
**String**: character sequence.  
**String Literal**: character sequence surrounded by quotes.
**Whitespace Character**: Space, tabs, newline. `userString = scnr.next()` skips first whitespace and then stops at the next whitespace.  
`userString = scnr.next()` excludes whitespace. `userString = scnr.nextLine()` gets whitespace.  


