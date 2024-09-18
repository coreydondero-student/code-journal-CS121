# Enum Experimentation
Add the following code to the end of main:
`boolean result = Flavor.HUCKLEBERRY.ordinal() > Flavor.CHOCOLATE.ordinal();
System.out.printf("\n\n%s is greater than %s: %b\n",Flavor.HUCKLEBERRY, Flavor.CHOCOLATE, result);`

**Result: ** `HUCKLEBERRY is greater than CHOCOLATE: true` funny because this means huckleberry is actually
further down the list than chocolate. In my experience, #1 in a list is usually best.
