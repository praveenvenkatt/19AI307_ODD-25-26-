# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

## AIM:
To write a Java program that demonstrates stream chaining by using a BufferedReader wrapped over an InputStreamReader which is further wrapped over System.in.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required classes (java.io.*).

Step 3: Create an InputStreamReader object using System.in.

Step 4: Wrap the InputStreamReader with a BufferedReader.

Step 5: Use the BufferedReader to read input from the user.

Step 6: Print the input received to demonstrate successful stream chaining.

Step 7: End the program after closing the streams if needed.





## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class UserDetails 
{
    public static void main(String[] args) throws IOException 
    {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));

        String name = br.readLine();
        int age = Integer.parseInt(br.readLine());

        System.out.println("--- User Details ---");
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}


```






## OUTPUT:
<img width="698" height="473" alt="{59BFA6E3-4D5A-485A-B14C-8B3144498B86}" src="https://github.com/user-attachments/assets/7969287c-5c78-4b29-93b6-0943bdbb742c" />



## RESULT:
The program successfully demonstrates chaining of streams using BufferedReader → InputStreamReader → System.in.


