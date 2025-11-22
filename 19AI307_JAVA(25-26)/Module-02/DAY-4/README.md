# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a program to access a static variable using both class name and object.

## AIM:
To write a Java program that demonstrates accessing a static variable using both the class name and an object of the class.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a class and declare a static variable inside it.

Step 3: In the same class or another class, create the main method.

Step 4: Access the static variable directly using the class name.

Step 5: Create an object of the class.

Step 6: Access the same static variable using the created object.

Step 7: Print both values and end the program.





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class StaticVariableDemo 
{
    static int value;

    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        value = sc.nextInt();

        System.out.println("Accessing using class name: " + StaticVariableDemo.value);

        StaticVariableDemo obj = new StaticVariableDemo();
        System.out.println("Accessing using object: " + obj.value);
    }
}

```



## OUTPUT:
<img width="826" height="302" alt="{B6BB698B-67F3-4B4F-82C7-B742BF01B3D6}" src="https://github.com/user-attachments/assets/6b047644-9065-4c09-8ff5-de7bec75b05f" />



## RESULT:
The program successfully accesses the static variable using both the class name and an object, demonstrating how static members belong to the class.


