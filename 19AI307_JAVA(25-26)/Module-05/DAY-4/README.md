# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a java program for determine the priority and name of the current thread.

Note : Read the threadname from the User


## AIM:
To write a Java program that reads a thread name from the user, sets it to the current thread, and displays the thread’s name and priority.


## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.util).

Step 3: Read the thread name from the user.

Step 4: Get the reference of the current thread using Thread.currentThread().

Step 5: Set the name of the current thread using setName().

Step 6: Retrieve the thread’s name and priority using getName() and getPriority().

Step 7: Print the thread name and priority, then end the program.





## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.io.*;

public class ThreadInfo 
{
    public static void main(String[] args) throws IOException 
    {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        String threadName = br.readLine();

        Thread t = Thread.currentThread();
        t.setName(threadName);             

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t); 
    }
}

```






## OUTPUT:



## RESULT:
The program successfully reads a thread name from the user and displays the current thread's updated name and its default priority.

