# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
 Write a Java program to create a class called “Book” with private instance variables title, author, and price. Provide public getter and setter methods to access and modify these variables. Add a method called applyDiscount() that takes a percentage as a parameter and reduces the price by that percentage.

## AIM:
To write a Java program that creates a Book class with private variables and public getter/setter methods, and includes a method applyDiscount() to reduce the book price by a given percent

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a class named Book with private variables: title, author, and price.

Step 3: Write public getter and setter methods for each variable.

Step 4: Create a method applyDiscount(double percent) that calculates the discount amount.

Step 5: Subtract the discount amount from the original price to update the price.

Step 6: In the main method, create an object of the Book class and set the values using setter methods.

Step 7: Call the applyDiscount() method, then print the updated details and end the program.




## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Book {
    private String title;
    private String author;
    private double price;

    public String getTitle() {
        return title;
    }
    public String getAuthor() {
        return author;
    }
    public double getPrice() {
        return price;
    }

    public void setTitle(String title) {
        this.title = title;
    }
    public void setAuthor(String author) {
        this.author = author;
    }
    public void setPrice(double price) {
        this.price = price;
    }

    public void applyDiscount(double percentage) {
        if (percentage > 0 && percentage <= 100) {
            price = price - (price * (percentage / 100));
        }
    }

    public void display() {
        System.out.println("Title: " + title);
        System.out.println("Author: " + author);
        System.out.printf("Discounted Price: %.2f\n", price);
        System.out.println("-------------------------");
    }
}


public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Book book = new Book();

        book.setTitle(sc.nextLine());

        book.setAuthor(sc.nextLine());

        book.setPrice(sc.nextDouble());

        double discount = sc.nextDouble();

        book.applyDiscount(discount);

        book.display();

    }
}

```


## OUTPUT:
<img width="1001" height="581" alt="{A49CEE0C-59EB-43E5-8DCB-4584A0CB2BDF}" src="https://github.com/user-attachments/assets/7dfd2f7c-809f-4c26-bd95-f467d61f644a" />



## RESULT:
The program successfully creates a Book class with encapsulation, applies a discount to the price, and displays the updated book details.

