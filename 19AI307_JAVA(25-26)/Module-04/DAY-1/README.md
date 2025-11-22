# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
Write a program that reads two integers and divides the first by the second. Handle the case when division by zero occurs.

## AIM:
To write a Java program that reads two integers, performs division, and handles division-by-zero using exception handling.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read two integers from the user.

Step 4: Use a try block to perform division of the first number by the second.

Step 5: Catch the ArithmeticException that occurs when the second number is zero.

Step 6: Inside the catch block, print an appropriate message like “Cannot divide by zero”.

Step 7: End the program after printing the result or error message.





## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class DivisionExample 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        try 
        {
            int a = sc.nextInt();
            int b = sc.nextInt();
            int result = a / b;
            System.out.println("Result: " + result);
        } 
        catch (ArithmeticException e) 
        {
            System.out.println("Error: Division by zero");
        } 
        catch (Exception e) 
        {
            System.out.println("Error: Please enter valid integers.");
        }
        sc.close();
    }
}

```







## OUTPUT:
<img width="685" height="293" alt="{CDBBE3A5-4DC3-4DF4-98FA-A43A7BDCAA6D}" src="https://github.com/user-attachments/assets/d44b016b-425c-4f67-931b-9c9a2021de81" />



## RESULT:
The program successfully performs division and handles division-by-zero errors using exception handling.



