# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade based on the marks:

Marks ≥ 90: Grade A

Marks ≥ 75 and < 90: Grade B

Marks ≥ 50 and < 75: Grade C

Marks < 50: Grade F


## AIM:
To write a Java program that demonstrates inheritance by creating a superclass Person and a subclass Student, and calculates the student’s grade based on marks.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a superclass Person with fields name and age.

Step 3: Create a subclass Student that extends Person and adds a field marks.

Step 4: Inside the Student class, implement the method calculateGrade() to check the marks.

Step 5: Use conditional statements to return grades A, B, C, or F based on marks.

Step 6: In the main method, create an object of the Student class and assign values to its fields.

Step 7: Call the calculateGrade() method, print the grade, and end the program.



## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by:  Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Person 
{
    String name;
    int age;

    public Person(String name, int age) 
    {
        this.name = name;
        this.age = age;
    }

    public void displayPersonInfo() 
    {
        System.out.println("Name: " + name + "\nAge: " + age);
    }
}

class Student extends Person 
{
    int marks;

    public Student(String name, int age, int marks) 
    {
        super(name, age); 
        this.marks = marks;
    }

    public String calculateGrade() 
    {
        if (marks >= 90) 
        {
            return "Grade: A";
        } 
        else if (marks >= 75) 
        {
            return "Grade: B";
        } 
        else if (marks >= 50) 
        {
            return "Grade: C";
        } 
        else 
        {
            return "Grade: F";
        }
    }

    public void displayStudentInfo() 
    {
        displayPersonInfo(); 
        System.out.println("Marks: " + marks);
        System.out.println(calculateGrade());
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();

        int age = sc.nextInt();

        int marks = sc.nextInt();

        Student s = new Student(name, age, marks);

        s.displayStudentInfo();

    }
}

```






## OUTPUT:
<img width="556" height="574" alt="{488A2736-CB9E-4364-BC63-FA681BCA4239}" src="https://github.com/user-attachments/assets/7ae8069d-d516-4f32-b126-630dad022851" />



## RESULT:
The program successfully demonstrates inheritance and calculates the student’s grade based on the marks provided.


