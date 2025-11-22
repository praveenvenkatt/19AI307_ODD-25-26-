# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Calculator with: One non-static method add(int a, int b) that returns the sum, One static method info() that says "Calculator is ready".


## AIM:
To write a Java program that creates a Calculator class with a non-static add() method for addition and a static info() method that prints a message.


## ALGORITHM :
Step 1: Start the program.

Step 2: Create a class named Calculator.

Step 3: Define a non-static method add(int a, int b) that returns the sum of two numbers.

Step 4: Define a static method info() that prints "Calculator is ready".

Step 5: In the main method, call the static method info() using the class name.

Step 6: Create an object of the Calculator class.

Step 7: Use the object to call the add() method, print the result, and end the program.




## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Calculator 
{
    public int add(int a, int b) 
    {
        return a + b;
    }

    public static void info() 
    {
        System.out.println("Calculator is ready");
    }
}

class prog 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();

        Calculator.info();

        Calculator obj = new Calculator();
        int sum = obj.add(a, b);
        System.out.println("Sum: " + sum);
    }
}

```



## OUTPUT:
<img width="645" height="323" alt="{E9C4626B-BA84-4EEC-A437-C0429DE1DBCD}" src="https://github.com/user-attachments/assets/f80e6a1f-6065-4d00-9331-2c1cf974c563" />



## RESULT:
The program successfully demonstrates the use of both static and non-static methods in the Calculator class.

