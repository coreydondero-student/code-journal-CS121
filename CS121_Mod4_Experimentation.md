# Static Method Experimentation
1.  
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
2.  
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
