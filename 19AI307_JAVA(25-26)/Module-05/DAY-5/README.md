# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Maintain two int variables a and b, read their initial values from user. Use synchronized block to swap them and print swapped values.

Input:

Two lines: a and b values

Output:

a = <swapped_a>

b = <swapped_b>

## AIM:
To write a Java program that reads two integers from the user and uses a synchronized block to swap their values and display the swapped result.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package java.util.*.

Step 3: Read two integer values a and b from the user.

Step 4: Create a shared lock object for synchronization.

Step 5: Use a synchronized block with the lock to safely swap the values of a and b.

Step 6: Print the swapped values of a and b.

Step 7: End the program.

## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.io.*;

public class SwapSync 
{
    public static void main(String[] args) throws IOException 
    {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));

        int a = Integer.parseInt(br.readLine());
        int b = Integer.parseInt(br.readLine());

        Object lock = new Object();

        synchronized (lock) 
        {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
}

```






## OUTPUT:
<img width="404" height="322" alt="{7179803E-66A4-446F-8DE1-EC2FE43E7634}" src="https://github.com/user-attachments/assets/a66076ec-fb0c-461d-90af-cf8262ec3215" />



## RESULT:
Thus, the program to swap two integers using a synchronized block was executed successfully.


