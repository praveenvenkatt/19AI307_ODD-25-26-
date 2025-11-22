# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is learning java basics, can you teach her the different types of datatypes in java? Write a program that uses all datatypes and print them all.

Input Format:

byte - 24

short - 11000

int - 1,34,500

long - 24,23,10,34

float - 24.20

double - 1,30,000.80

boolean - true/false

char - 'u'

String -"Heyyy, Lovely, Let's learn java!"



## AIM:
To understand and demonstrate the different data types in Java by creating a program that declares variables of all data types and prints their values.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Declare variables for all primitive datatypes (byte, short, int, long, float, double, boolean, char).

Step 4: Declare a variable for the non-primitive datatype (String).

Step 5: Assign the given input values to all the declared variables.

Step 6: Print all variable values using System.out.println().

Step 7: Stop/End the program.



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Praveen V
RegisterNumber: 212222040121
*/
```

## Sourcecode.java:
```
import java.util.*;

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);

        byte b = sc.nextByte();
        short s = sc.nextShort();
        int i = sc.nextInt();
        long l = sc.nextLong();
        float f = sc.nextFloat();
        double d = sc.nextDouble();
        boolean bool = sc.nextBoolean();
        char c = sc.next().charAt(0);
        sc.nextLine();
        String str = sc.nextLine();

        System.out.println("Hey Lovely, let's print all types of data received from user using different data types");

        System.out.println("This is byte datatype " + b);
        System.out.println("This is short datatype " + s);
        System.out.println("This is int datatype " + i);
        System.out.println("This is long datatype " + l);
        System.out.println("This is float datatype " + f);
        System.out.println("This is double datatype " + d);
        System.out.println("This is boolean datatype " + bool);
        System.out.println("This is char datatype " + c);
        System.out.println("This is string datatype " + str);
    }
}

```


## OUTPUT:
<img width="975" height="601" alt="{455D9E73-3A20-4AB6-AA8B-DC7A9C1DC8F5}" src="https://github.com/user-attachments/assets/a15cfc5b-14f7-45ea-bd3a-e8fa568c9b52" />
<img width="850" height="571" alt="{1524A778-8B3C-40F7-AC61-62FB28084911}" src="https://github.com/user-attachments/assets/d19eaaa1-385e-432c-b3f2-c7480424631d" />






## RESULT:
The program successfully demonstrates all Java data types by declaring, assigning, and printing each of them.







