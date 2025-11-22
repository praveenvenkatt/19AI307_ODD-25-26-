# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.



## AIM:
To write a Java program that reverses a given string using a loop.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read a string input from the user.

Step 4: Create an empty string rev to store the reversed result.

Step 5: Use a loop to traverse the original string from the last character to the first.

Step 6: Append each character to the rev string.

Step 7: Print the reversed string and end the program.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseString 
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        String str = sc.nextLine();
        String reversed = "";

        for (int i = str.length() - 1; i >= 0; i--) 
        {
            reversed += str.charAt(i);
        }

        System.out.println("Reversed string: " + reversed);
    }
}

```
## OUTPUT:
<img width="697" height="254" alt="{C3EF4677-42C3-4160-BA28-5DCA823235F1}" src="https://github.com/user-attachments/assets/df6e1f39-e499-44d7-bf60-2bc4c9f17a22" />






## RESULT:
The program successfully reverses the given string and displays the reversed output.







