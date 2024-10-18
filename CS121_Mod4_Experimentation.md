# Static Method Experimentation
## 1.  
**Add the following code to utility.java:**  
```
public static void numDoubler1(int x) {
    x = x * 2;
}

public static int numDoubler2(int x) {
    x = x * 2;
    return x;
}
```
**Add the following to StaticFun.java**  
```
int myNum = 2;

Utility.numDoubler1(myNum);
System.out.println("Value of myNum after calling numDoubler1: " + myNum);

myNum = Utility.numDoubler2(myNum);
System.out.println("Value of myNum after calling numDoubler2: " + myNum);
```
**What happened?**  
numDoubler1 did not double the number because it did not return anything. numDoubler2 did work because it returned the value after doubling.  
## 2.  
**Add the following to utility.java**  
```
public static void pointDoubler(Point p) {
    p.x = p.x * 2;
    p.y = p.y * 2;
}
```
**Add the following to StaticFun.java**  
```
Point myPoint = new Point(2,3);

System.out.println("Value of point before doubling: " + myPoint);
Utility.pointDoubler(myPoint);
System.out.println("Value of point after doubling: " + myPoint);\
```
**What happened?**  
Were the values of x and y inside the Point object modified by the pointDoubler() method even though it doesn't have a return value? What is the difference between passing in an object as a argument to a method vs passing in a primitive data type such as an int?  

The values in Poitn were modified because we passed the argument as an object instead of a primitive data type.  

# ArrayList Experimentation
## 1. 
**Add the following to MyRainbow.java**
```
rainbow.add(Color.GREEN);
rainbow.add(Color.BLUE);
rainbow.add(Color.BLACK);
```
**What happened?**  
As expected the list is 3 longer, so 6. New colors were added in the order which the code ran.  
## 2.
**Add a non color object to the array**  
`rainbow.add("Purple");`  
**What happened?**  
Code did not compile. Stack trace says: "The method add(Color) in the type ArrayList<Color> is not applicable for the arguments (String)"  
## 3. 
Change the rainbow.remove(0) line to `rainbow.remove(199)`.  
**What happened?**
```
Exception in thread "main" java.lang.IndexOutOfBoundsException: Index 199 out of bounds for length 3
        at java.base/jdk.internal.util.Preconditions.outOfBounds(Preconditions.java:64)
        at java.base/jdk.internal.util.Preconditions.outOfBoundsCheckIndex(Preconditions.java:70)
        at java.base/jdk.internal.util.Preconditions.checkIndex(Preconditions.java:266)
        at java.base/java.util.Objects.checkIndex(Objects.java:361)
        at java.base/java.util.ArrayList.remove(ArrayList.java:504)
        at MyRainbow.main(MyRainbow.java:33)
```
# File parsing experimentation
## 1.
**Modify the display code in FileEcho.java like so:**  
```
int lineNumber = 1;
while (fileScan.hasNextLine()) {
    String line = fileScan.nextLine();

    System.out.printf("%5d | %s\n",lineNumber,line);

    lineNumber++;
}
```
**What happened?**  
the code prepended with a line number. it seems to match the line numbers in my java files. Works on the Jimmy Buffett Bill of Rights files.  
## 2. 
**Modify the existing loop in CSVParser.java to prepend line numbers**
```
    /* 3. Create a loop to read each line from the Scanner */
    int lineNumber = 1;
    while(bobsScanner.hasNextLine()) {
        String line = bobsScanner.nextLine();

        /* 4. Print each line */
        System.out.printf("Processing Line %3d: %s\n",lineNumber,line);
        lineNumber++;
```
