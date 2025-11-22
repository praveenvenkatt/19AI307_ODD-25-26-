# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Car with attributes brand, model, year. Create 2 objects and print their details.

For example:

Result
Car 1: Toyota Innova 2022
Car 2: Hyundai i20 2021



## AIM:
To write a Java program that creates a Car class with attributes brand, model, and year, creates two objects of the class, and prints their details.


## ALGORITHM :
Step 1: Start the program.

Step 2: Create a class named Car with attributes brand, model, and year.

Step 3: Define a constructor to initialize the car attributes.

Step 4: Inside the main method, create two objects of the Car class.

Step 5: Assign brand, model, and year values to both objects using the constructor.

Step 6: Print the details of both car objects.

Step 7: End the program.





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by:  Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```

public class Main
{
    static class Car
    {
        String brand;
        String model;
        int year;
    }

    public static void main(String[] args)
    {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}

```


## OUTPUT:
<img width="595" height="170" alt="{726BA8F1-A3FE-4D87-B2D0-57B66332F34D}" src="https://github.com/user-attachments/assets/5ef98e90-59aa-4c92-9bba-6e1eabd001e0" />



## RESULT:
The program successfully creates two car objects and prints their brand, model, and manufacturing year.


