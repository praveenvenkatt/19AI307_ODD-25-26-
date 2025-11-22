# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Write a Java program to create a new file named example.txt.

## AIM:
To write a Java program that creates a new file named example.txt using Java’s file handling classes.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package (java.io).

Step 3: Create a File object with the filename "example.txt".

Step 4: Use the createNewFile() method to create the file.

Step 5: Check if the file is successfully created.

Step 6: Print an appropriate message indicating success or failure.

Step 7: End the program.





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.io.File;
import java.io.IOException;

public class CreateFileExample 
{
    
    static void createFile() 
    {
        try 
        {
            File file = new File("example.txt");

            if (file.createNewFile()) 
            {
                System.out.println("File created: " + file.getName());
            } 
            else 
            {
                System.out.println("File already exists.");
            }

        } 
        catch (IOException e) 
        {
            System.out.println("An error occurred.");
        }
    }

    public static void main(String[] args) 
    {
        createFile();
    }
}

```






## OUTPUT:
<img width="633" height="150" alt="{1D965F97-986D-4C05-8A02-18E2D3D6E17B}" src="https://github.com/user-attachments/assets/40857695-72a6-4e75-aaf9-670affde2b6c" />



## RESULT:
The program successfully creates a new file named example.txt in the project directory.



