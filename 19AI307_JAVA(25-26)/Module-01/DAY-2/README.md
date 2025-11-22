# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
In a magical building, an elevator behaves oddly:

If the floor number is divisible by 3 and 5, it says "Skipped".

If the floor number is divisible by 3 only, it says "Beware!".

If the floor number is divisible by 5 only, it says "Blessings!".

Otherwise, it announces the floor number - print - "Floor {number}" .

Write a Java program to simulate this elevator logic for a given floor number.


## AIM:
To write a Java program that simulates the special elevator logic by checking the given floor number and printing the appropriate message based on divisibility rules.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read the input floor number from the user.

Step 4: Check if the number is divisible by both 3 and 5; if true, print "Skipped".

Step 5: Otherwise, check if it is divisible by 3; if true, print "Beware!".

Step 6: Otherwise, check if it is divisible by 5; if true, print "Blessings!".

Step 7: If none of the conditions match, print "Floor {number}" and end the program.


## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

public class MagicalElevator
{
    
    public static void elevatorMessage(int floor)
    {
        if (floor % 3 == 0 && floor % 5 == 0)
        {
            System.out.println("Skipped");
        } 
        else if (floor % 3 == 0)
        {
            System.out.println("Beware!");
        } 
        else if (floor % 5 == 0)
        {
            System.out.println("Blessings!");
        } 
        else
        {
            System.out.println("Floor " + floor);
        }
    }

    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int floor = sc.nextInt();
        elevatorMessage(floor);
        sc.close();
    }
}


```





## OUTPUT:
<img width="493" height="280" alt="{77C4104B-A8F3-4FC4-943C-D8386CE56D59}" src="https://github.com/user-attachments/assets/3f62dcf1-3e38-45f7-b0dc-4e3148c3331f" />







## RESULT:
The program successfully simulates the magical elevator by printing the correct message based on the floor number entered.








