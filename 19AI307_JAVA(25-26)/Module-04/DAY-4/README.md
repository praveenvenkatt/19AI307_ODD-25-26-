# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
You’re creating a cross-platform UI tool using the Abstract Factory pattern. Implement factories to create Button and Checkbox for "dark" and "light" themes. Let the user choose the theme, then generate UI components and display their types

## AIM:
To implement the Abstract Factory design pattern in Java to create UI components (Button and Checkbox) for two themes—dark and light—based on the user’s selection.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create interfaces for Button and Checkbox with a method to display their type.

Step 3: Create concrete classes for DarkButton, LightButton, DarkCheckbox, and LightCheckbox.

Step 4: Create an abstract factory interface with methods to create a Button and a Checkbox.

Step 5: Implement two factory classes: DarkThemeFactory and LightThemeFactory, each returning theme-specific components.

Step 6: Read the user’s choice (dark or light) and create the corresponding factory object.

Step 7: Use the factory to generate Button and Checkbox objects, display their types, and end the program.





## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

interface Button 
{
    void paint();
}

interface Checkbox 
{
    void paint();
}

class DarkButton implements Button 
{
    public void paint() 
    {
        System.out.println("Dark Button created");
    }
}

class DarkCheckbox implements Checkbox 
{
    public void paint() 
    {
        System.out.println("Dark Checkbox created");
    }
}

class LightButton implements Button 
{
    public void paint() 
    {
        System.out.println("Light Button created");
    }
}

class LightCheckbox implements Checkbox 
{
    public void paint() 
    {
        System.out.println("Light Checkbox created");
    }
}

interface UIFactory 
{
    Button createButton();
    Checkbox createCheckbox();
}

class DarkFactory implements UIFactory 
{
    public Button createButton() 
    {
        return new DarkButton();
    }

    public Checkbox createCheckbox() 
    {
        return new DarkCheckbox();
    }
}

class LightFactory implements UIFactory 
{
    public Button createButton() 
    {
        return new LightButton();
    }

    public Checkbox createCheckbox() 
    {
        return new LightCheckbox();
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        String theme = sc.nextLine().trim();

        UIFactory factory;

        if (theme.equalsIgnoreCase("dark")) 
        {
            factory = new DarkFactory();
        } 
        else if (theme.equalsIgnoreCase("light")) 
        {
            factory = new LightFactory();
        } 
        else 
        {
            System.out.println("Invalid theme");
            sc.close();
            return;
        }
        factory.createButton().paint();
        factory.createCheckbox().paint();
    }
}

```






## OUTPUT:
<img width="823" height="290" alt="{EB73B6DF-CACF-4FB5-9504-6964F938E3FF}" src="https://github.com/user-attachments/assets/76fbf811-b183-45b4-9f77-bad2d17325a6" />



## RESULT:
The program successfully implements the Abstract Factory pattern by generating Button and Checkbox components according to the user-selected theme (dark or light).


