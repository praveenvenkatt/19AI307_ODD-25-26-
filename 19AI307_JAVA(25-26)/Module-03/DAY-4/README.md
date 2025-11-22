# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.


 Bot Types:

SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".

RainBot: Predicts "COLD" if temperature < 20, else "WARM".

Input:

temperature
botType (1 for SunBot, 2 for RainBot)Output:
Prediction as a string.

## AIM:
To write a Java program where different weather bots implement a common interface and give predictions based on temperature and bot type.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create an interface with a method predict(int temperature).

Step 3: Implement the interface in a SunBot class that returns "HOT" if temperature > 30, otherwise "MODERATE".

Step 4: Implement the interface in a RainBot class that returns "COLD" if temperature < 20, otherwise "WARM".

Step 5: Read the temperature and bot type as input.

Step 6: Based on bot type, create either a SunBot or RainBot object.

Step 7: Call the predict() method and print the prediction, then end the program.


## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface WeatherBot 
{
    String predict(int temperature);
}

class SunBot implements WeatherBot 
{
    @Override
    public String predict(int temperature) 
    {
        return (temperature > 30) ? "HOT" : "MODERATE";
    }
}

class RainBot implements WeatherBot 
{
    @Override
    public String predict(int temperature) 
    {
        return (temperature < 20) ? "COLD" : "WARM";
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int temperature = sc.nextInt();
        int botType = sc.nextInt();

        WeatherBot bot;
        if (botType == 1) 
        {
            bot = new SunBot();
        } 
        else 
        {
            bot = new RainBot();
        }

        System.out.println(bot.predict(temperature));
    }
}

```






## OUTPUT:
<img width="440" height="168" alt="{6D227532-E04D-4764-AC36-1801DFCA66CB}" src="https://github.com/user-attachments/assets/b0f6a242-6a33-4cc6-bdae-15af5c904999" />



## RESULT:
The program successfully predicts weather conditions using the chosen bot based on the given temperature.


