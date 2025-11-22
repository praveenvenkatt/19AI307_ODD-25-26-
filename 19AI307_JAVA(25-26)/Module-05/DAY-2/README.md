# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:
Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.

## AIM:
To write a Java program that serializes a collection of objects, such as an ArrayList<Student>, and stores it into a file using Object Serialization.

## ALGORITHM :
Step 1: Start the program.

Step 2: Import the required classes (java.io.* and java.util.*).

Step 3: Create a Student class that implements Serializable.

Step 4: Create an ArrayList<Student> and add multiple Student objects to it.

Step 5: Create a FileOutputStream to open a file for writing serialized data.

Step 6: Wrap the FileOutputStream inside an ObjectOutputStream and write the ArrayList<Student> to the file.

Step 7: Close the streams, finish serialization, and end the program.





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

class Student implements Serializable 
{
    private static final long serialVersionUID = 1L;

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) 
    {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    @Override
    public String toString() 
    {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class StudentSerializationUserInput 
{

    public static void serializeStudents(List<Student> students, String fileName) 
    {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream(fileName))) 
        {
            oos.writeObject(students);
            System.out.println("Students serialized successfully into: " + fileName);
        } 
        catch (IOException e) 
        {
            System.out.println("Error during serialization: " + e.getMessage());
        }
    }

    @SuppressWarnings("unchecked")
    public static List<Student> deserializeStudents(String fileName) 
    {
        List<Student> students = null;
        try (ObjectInputStream ois = new ObjectInputStream(new FileInputStream(fileName))) 
        {
            students = (List<Student>) ois.readObject();
            System.out.println("Students deserialized successfully from: " + fileName);
        } 
        catch (IOException | ClassNotFoundException e) 
        {
            System.out.println("Error during deserialization: " + e.getMessage());
        }
        return students;
    }

    public static void main(String[] args) 
    {
        Scanner scanner = new Scanner(System.in);
        List<Student> students = new ArrayList<>();

        int n = scanner.nextInt();
        scanner.nextLine();

        for (int i = 0; i < n; i++) 
        {
            int id = scanner.nextInt();
            scanner.nextLine(); 
            String name = scanner.nextLine();
            double marks = scanner.nextDouble();
            if (i != n - 1) scanner.nextLine(); 

            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        serializeStudents(students, fileName);

        List<Student> deserializedStudents = deserializeStudents(fileName);

        if (deserializedStudents != null) 
        {
            System.out.println("\nDeserialized Students:");
            for (Student s : deserializedStudents) 
            {
                System.out.println(s);
            }
        }
    }
}

```






## OUTPUT:
<img width="1174" height="428" alt="{A75CC715-07DA-470D-802E-576A93CCA983}" src="https://github.com/user-attachments/assets/d437c419-d810-4283-a695-55611a5a6693" />



## RESULT:
The program successfully serializes a collection of Student objects and stores them into a file using Java object serialization.


