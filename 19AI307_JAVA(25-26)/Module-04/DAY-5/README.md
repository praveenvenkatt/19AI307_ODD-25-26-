# Ex.No:4(E) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
You need to clone documents. Implement the Prototype Pattern to copy a Document object with a title and content. On user input, create a copy and print both the original and the clone.

## AIM:
To implement the Prototype Design Pattern in Java by creating a Document object that can clone itself, and demonstrate cloning using user input.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required package java.util.* for user input.

Step 3: Create a Document class that implements Cloneable and contains title and content fields.

Step 4: Override the clone() method to return a copied Document object.

Step 5: In the main program, read the title and content from the user.

Step 6: Create the original Document object, clone it using the prototype method, and store the cloned object.

Step 7: Print the original and cloned Document values, then end the program.





## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

interface Prototype 
{
    Prototype clone();
}

class Document implements Prototype 
{
    private String title;
    private String content;

    public Document(String title, String content) 
    {
        this.title = title;
        this.content = content;
    }

    public void display(String type) 
    {
        System.out.println(type + ": " + title + " - " + content);
    }

    @Override
    public Prototype clone() 
    {
        return new Document(this.title, this.content);
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);

        String title = sc.nextLine();
        String content = sc.nextLine();

        Document original = new Document(title, content);
        Document cloned = (Document) original.clone();

        original.display("Original");
        cloned.display("Cloned");
    }
}

```






## OUTPUT:
<img width="1245" height="292" alt="{0DF2E984-C263-46B7-80CC-A849673DC2EF}" src="https://github.com/user-attachments/assets/1e901c46-176f-4055-a32f-d21af2fd3e1e" />



## RESULT:
Thus, the program successfully cloned a Document object using the Prototype Pattern and displayed both the original and copied versions.



