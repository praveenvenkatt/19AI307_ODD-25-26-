# Ex.No:3(E) INNER CLASS

## QUESTION:
 Write a Java program where the inner class is declared private and accessed through a method in the outer class. 

## AIM:
To write a Java program where a private inner class is declared inside an outer class and accessed using a public method of the outer class.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create an outer class named Outer.

Step 3: Inside the outer class, declare a private inner class named Inner.

Step 4: Define a method inside the private inner class to display a message.

Step 5: In the outer class, create a public method to create an object of the private inner class.

Step 6: From this method, access the private inner class and call its method.

Step 7: In the main method, create an object of Outer and call the method that accesses the private inner class.





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.*;

class Outer 
{
    private class Inner 
    {
        int num;
        Inner(int n) 
        {
            num = n;
        }
        void display() 
        {
            System.out.println("Data set inside private inner class: " + num);
        }
    }

    void accessInner(int n) 
    {
        Inner in = new Inner(n);
        in.display();
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        Outer out = new Outer();
        out.accessInner(n);
    }
}

```






## OUTPUT:
<img width="961" height="241" alt="{B1964C5C-A34E-4C76-B72B-96DE23096B13}" src="https://github.com/user-attachments/assets/e0576564-908d-47ec-92d1-9d29e21e0580" />



## RESULT:
Thus, the program to access a private inner class through a method in the outer class was successfully implemented.
