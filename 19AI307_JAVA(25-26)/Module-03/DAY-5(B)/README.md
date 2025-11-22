# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.


## AIM:
To write a Java program that checks whether a given number is an Armstrong number using Math.pow() and the Integer wrapper class.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read an integer input from the user using the Integer wrapper class.

Step 4: Convert the number to a string to count its digits.

Step 5: Use a loop to extract each digit and calculate the sum of digits raised to the power of total digits using Math.pow().

Step 6: Compare the calculated sum with the original number.

Step 7: Print whether the number is an Armstrong number and end the program.



## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();

        int digits = Integer.toString(num).length(); 
        int sum = 0, temp = num;

        while (temp > 0) 
        {
            int digit = temp % 10;
            sum += (int)Math.pow(digit, digits); 
            temp /= 10;
        }

        if (sum == num) 
        {
            System.out.println(num + " is an Armstrong number.");
        } 
        else 
        {
            System.out.println(num + " is not an Armstrong number.");
        }
    }
}

```






## OUTPUT:
<img width="904" height="248" alt="{8C7949A3-EAC0-45CE-AFDE-1FBC0CAE1410}" src="https://github.com/user-attachments/assets/68ccbdc0-052a-4dc9-916b-d1e0e09bc9a1" />



## RESULT:
The program successfully checks and displays whether the input number is an Armstrong number.


