# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.



## AIM:
To write a Java program that calculates the factorial of a given number using a for loop.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read an integer input from the user.

Step 4: Initialize a variable fact to 1.

Step 5: Use a for loop to multiply all numbers from 1 to the given number.

Step 6: Store the final multiplication result in the fact variable.

Step 7: Print the factorial value and end the program.


## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

public class prog
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int fact=1;
        
        for(int i=1;i<=n;i++)
        {
            fact=fact*i;
        }
        System.out.print("Factorial of "+n+" is: "+fact);
    }
}
```



## OUTPUT:
<img width="707" height="242" alt="{9536360F-6F59-420E-BF27-E5018BD5B0AA}" src="https://github.com/user-attachments/assets/9918bb8a-61ef-408f-aff7-ffa37537cac9" />





## RESULT:
The program successfully calculates and displays the factorial of the given number using a for loop.






