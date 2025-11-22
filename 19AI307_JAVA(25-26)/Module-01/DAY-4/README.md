# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java Program to Find the Average of Array Elements.




## AIM:
To write a Java program that finds the average of the elements in an array by summing all elements and dividing by the total count.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read the size of the array from the user.

Step 4: Declare an array and input all its elements.

Step 5: Initialize a variable sum to 0.

Step 6: Use a loop to add each array element to sum.

Step 7: Calculate the average using sum / number_of_elements and print the result.





## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Praveen V
RegisterNumber: 212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int arr[] = new int[n];
        
        for (int i = 0; i < n; i++) 
        {
            arr[i] = sc.nextInt();
        }
        
        float sum = 0;
        for (int i = 0; i < n; i++) 
        {
            sum += arr[i];
        }
        float avg = sum / n;
        System.out.printf("The average of elements is %.2f", avg);
    }
}

```

## OUTPUT:
<img width="774" height="467" alt="{FCB6CDC3-228C-439A-9360-E49B9E1F8B1C}" src="https://github.com/user-attachments/assets/6d9649c4-93e8-47b9-ada9-34fccf68189e" />





## RESULT:
The program successfully reads the array elements, calculates the total sum, and displays the average of the array.





