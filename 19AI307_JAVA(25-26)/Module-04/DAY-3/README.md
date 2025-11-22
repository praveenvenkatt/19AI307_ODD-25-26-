# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

## AIM:
To write a Java program demonstrating Composition by creating a Library class that contains multiple Book objects, where each Book is created inside the Library and cannot exist independently.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a Book class with attributes like title and author.

Step 3: Create a Library class that has a list or array of Book objects.

Step 4: Inside the Library constructor, create and initialize all Book objects (ensuring they cannot exist independently).

Step 5: Add a method to display all books in the library.

Step 6: In the main method, create a Library object.

Step 7: Call the display method to print all book details and end the program.



## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

class Book 
{
    private String title;
    private String author;

    public Book(String title, String author) 
    {
        this.title = title;
        this.author = author;
    }

    public String getDetails() 
    {
        return title + " by " + author;
    }
}

class Library 
{
    private List<Book> books;

    public Library() 
    {
        this.books = new ArrayList<>();
    }

    public void addBook(String title, String author) 
    {
        Book newBook = new Book(title, author);
        this.books.add(newBook);
    }

    public void showBooks() 
    {
        System.out.println("Books in Library:");
        for (Book book : this.books) 
        {
            System.out.println("- " + book.getDetails());
        }
    }
}

public class prog 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = 0;
        if (sc.hasNextInt()) 
        {
            n = sc.nextInt();
        }
        sc.nextLine();

        for (int i = 0; i < n; i++) 
        {
            if (!sc.hasNextLine()) break;
            String title = sc.nextLine().trim();
            if (!sc.hasNextLine()) break;
            String author = sc.nextLine().trim();
            library.addBook(title, author);
        }

        library.showBooks();

        int m = 0;
        if (sc.hasNextInt()) 
        {
            m = sc.nextInt();
        } 
        else 
        {
            sc.close();
            return;
        }
        sc.nextLine();
        
        for (int i = 0; i < m; i++) 
        {
            if (!sc.hasNextLine()) break;
            String title = sc.nextLine().trim();
            if (!sc.hasNextLine()) break;
            String author = sc.nextLine().trim();
            library.addBook(title, author);
            
            library.showBooks();
        }
    }
}

```






## OUTPUT:



## RESULT:
The program successfully demonstrates Composition by creating Book objects inside the Library, ensuring they depend entirely on the Library for their existence.

