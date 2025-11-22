# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).


## AIM:
To write a Java program that defines a method cube(int x) which internally calls another method square(int x) to compute the cube of a number.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a method square(int x) that returns the square of the given number.

Step 3: Create another method cube(int x) that calls square(x).

Step 4: Multiply x with the returned value of square(x) inside the cube method.

Step 5: Return the result from the cube method.

Step 6: In the main method, read or define a number to pass to the cube method.

Step 7: Print the cube value and end the program.



## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.*;

public class CubeCalculator 
{

    public int square(int x) 
    {
        return x * x;
    }

    public int cube(int x) 
    {
        return x * square(x);
    }

    public static void main(String[] args) 
    {
        CubeCalculator obj = new CubeCalculator();
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();      
        int result = obj.cube(num);  
        System.out.println(result);  
    }
}

```



## OUTPUT:
<img width="417" height="177" alt="{7B8E5DF0-893F-4DCC-B194-59E561272D41}" src="https://github.com/user-attachments/assets/2d23f391-be1d-4814-b508-50209162b565" />



## RESULT:
The program successfully calculates the cube of a number by internally calling the square method.


