# Enum Experimentation (IceCream.java)
**Add the following code to the end of main:**  
`boolean result = Flavor.HUCKLEBERRY.ordinal() > Flavor.CHOCOLATE.ordinal();
System.out.printf("\n\n%s is greater than %s: %b\n",Flavor.HUCKLEBERRY, Flavor.CHOCOLATE, result);`  
**Result:** `HUCKLEBERRY is greater than CHOCOLATE: true` funny because this means huckleberry is actually
further down the list than chocolate. In my experience, #1 in a list is usually best.  

**Modify the code to look like the following (\n to %n):**  
`System.out.printf("%n%n%s is greater than %s: %b%n",Flavor.HUCKLEBERRY, Flavor.CHOCOLATE, result);  
**Result:** Apparently there is not a difference?  

# Formatting Experimentation (CircleStatsDecimalFormat.java & BasicDecimalFormat.java)
**Add the following code to CircleStats:**  
`System.out.printf("The circle's area using printf(): %.4f\n", area);
System.out.printf("The circle's circumference using printf(): %10.3f\n", circumference);`  
**Result:**  
`The circle's area: 706.858  
The circle's circumference: 94.248  
The circle's area using printf(): 706.8583  
The circle's circumference using printf():     94.248`  
In the first change, the %.4f tells it to print a 4 decimal float.  
The second change has %10.3f, which is a 3 decimal float at least 10 characters long. 
The program adds whitespace for the extra characters.  

**modify the following code to BasicDecimal:**  
`DecimalFormat fmt = new DecimalFormat("$0.###");` to `DecimalFormat fmt = new DecimalFormat("$0.000");`  
**Result:** Forces an extra zero in the tax number. it's a two decimal float but this will print it as a 3 deimal float.  

**modify the following code to BasicDecimal:**  
`DecimalFormat fmt = new DecimalFormat("$0.000");` to `DecimalFormat fmt = new DecimalFormat("$00000.000000");`  
**Result:** Forces leading and trailing zeros to match the format.  

# String Experimentation (StringFun.java)
**Add a print statement to the index of the character in the console as shown below.**  
`System.out.println("Character index is: " + space);`  
**Result:** Prints 5, because the space is in position number 5.  

**Change the index character to one that doesn't exist in the phrase.**  
`int space = phrase.indexOf('z'); `  
**Result:** An error `Exception in thread "main" java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 11`  

# Random Experimentation (RandomNumbers.java)
**Try running three times as-is**  
**Result:** random numbers each time.  

**Instantiate the Random object using a seed value as shown below**  
`generator = new Random(12345);`  
**Result:** same numbers on each run.  

# Math Experimentation (Quadratic.java)
**Modify the program to support reading double values from the user by replacing the nextInt() methods calls with nextDouble() as shown below.**
`System.out.print("Enter the coefficient of x squared: ");
a = scan.nextDouble();
System.out.print("Enter the coefficient of x: ");
b = scan.nextDouble();
System.out.print("Enter the constant: ");
c = scan.nextDouble();`  
**Result:** Type mismatch error, won't compile. Can't put a double value in an int variable.  

**Modify the program by casting the value returned by nextDouble() to an int as shown below. Run the program with the values 2.5, 16.8, 3.2 for a, b and c respectively**  
`System.out.print("Enter the coefficient of x squared: ");
a = (int) scan.nextDouble();
System.out.print("Enter the coefficient of x: ");
b = (int) scan.nextDouble();
System.out.print("Enter the constant: ");
c = (int) scan.nextDouble();`  
**Result:**  same as before modification, because even though we have a double value, we cast it ot int, so the decimals are lost.  

**Remove the cast and change the declaration for a, b and c from int to double as shown below. Run the program with the values 2.5, 16.8, 3.2 for a, b and c respectively.**  
`double a, b, c;`  
**Result:** Now we have correct numbers because we used double the whole way through.
