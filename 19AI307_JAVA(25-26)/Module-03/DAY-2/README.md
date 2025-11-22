# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with:

area(int side) for square

area(int length, int breadth) for rectangle

area(double radius) for circle

## AIM:
To write a Java program that demonstrates method overloading by calculating the areas of a square, rectangle, and circle using different versions of the area() method.


## ALGORITHM :
Step 1: Start the program.

Step 2: Create a class named AreaCalculator.

Step 3: Overload the method area(int side) to calculate and return the area of a square.

Step 4: Overload the method area(int length, int breadth) to calculate and return the area of a rectangle.

Step 5: Overload the method area(double radius) to calculate and return the area of a circle.

Step 6: In the main method, create an object of AreaCalculator and call each overloaded method with appropriate values.

Step 7: Print the area results for square, rectangle, and circle and end the program.





## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class AreaCalculator 
{

    int area(int side) 
    {
        return side * side;
    }

    int area(int length, int breadth) 
    {
        return length * breadth;
    }

    double area(double radius) 
    {
        return Math.PI * radius * radius;
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        AreaCalculator ac = new AreaCalculator();
        int side = sc.nextInt();
        System.out.println("Area of square: " + ac.area(side));

        int length = sc.nextInt();
        int breadth = sc.nextInt();
        System.out.println("Area of rectangle: " + ac.area(length, breadth));

        double radius = sc.nextDouble();
        System.out.println("Area of circle: " + ac.area(radius));
    }
}

```






## OUTPUT:



## RESULT:
The program successfully calculates the areas of different shapes using method overloading.


