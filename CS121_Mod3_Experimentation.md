# Enum Experimentation (IceCream.java)
**Add the following code to the end of main:**  
`boolean result = Flavor.HUCKLEBERRY.ordinal() > Flavor.CHOCOLATE.ordinal();
System.out.printf("\n\n%s is greater than %s: %b\n",Flavor.HUCKLEBERRY, Flavor.CHOCOLATE, result);`  
**Result:** `HUCKLEBERRY is greater than CHOCOLATE: true` funny because this means huckleberry is actually
further down the list than chocolate. In my experience, #1 in a list is usually best.  

**Modify the code to look like the following (\n to %n):**  
`System.out.printf("%n%n%s is greater than %s: %b%n",Flavor.HUCKLEBERRY, Flavor.CHOCOLATE, result);  
**Result:** Apparently there is not a difference?  

# Formatting Experimentation (CircleStatsDecimalFormat.java)
**Add the followind code:**  
`System.out.printf("The circle's area using printf(): %.4f\n", area);
System.out.printf("The circle's circumference using printf(): %10.3f\n", circumference);`  
**Result:**  
`The circle's area: 706.858
The circle's circumference: 94.248
The circle's area using printf(): 706.8583
The circle's circumference using printf():     94.248`
