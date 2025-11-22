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
<img width="968" height="598" alt="{6E21FB16-7F1E-4250-9B20-498F32455158}" src="https://github.com/user-attachments/assets/537221f2-9dea-495b-8366-a4c489556d93" />
<img width="852" height="650" alt="{7C3F5E90-8FCC-4579-8654-01FAE053CAC6}" src="https://github.com/user-attachments/assets/a95a9e17-685c-4154-9cb9-67374ffe81e5" />



## RESULT:
The program successfully demonstrates all Java data types by declaring, assigning, and printing each of them.






