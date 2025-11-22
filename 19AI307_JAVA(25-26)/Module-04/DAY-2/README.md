# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:
In a gaming lounge, there is only one master console power switch that controls all gaming consoles. Whenever a player turns on any console, it internally triggers the master power. The master switch must ensure only one instance is ever created, regardless of how many times it's accessed, to prevent power fluctuations.

Every time a player accesses the master switch, it logs an access count. Since the switch is Singleton, the count should increment globally and reflect shared state.

Input Format:

n
[Player1]
[Player2]
...
First line: Integer n – number of players turning on consoles

Next n lines: Each line contains the player's name.

 

Output Format:
For each player, print:

[PlayerName] accessed Master Power Switch. Total accesses so far: [count]


## AIM:
To write a Java program that implements the Singleton design pattern for a master power switch, ensuring only one instance is created and maintaining a shared access count across multiple players.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create a Singleton class MasterSwitch with a private constructor and a static method to return the single instance.

Step 3: Add a private static variable to store the single instance and another variable to maintain the access count.

Step 4: Create a method access(String playerName) that increments the global access count.

Step 5: Read the number of players from the user.

Step 6: For each player name, obtain the same Singleton instance of MasterSwitch and call the access method.

Step 7: Print the player's name along with the updated global access count and end the program.





## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.*;

class MasterPowerSwitch 
{
    private static MasterPowerSwitch instance = null;
    private int accessCount = 0;

    private MasterPowerSwitch() 
    {
        
    }

    public static MasterPowerSwitch getInstance() 
    {
        if (instance == null) 
        {
            instance = new MasterPowerSwitch();
        }
        return instance;
    }

    public int logAccess() 
    {
        accessCount++;
        return accessCount;
    }
}

public class prog 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) 
        {
            String player = sc.nextLine();
            MasterPowerSwitch power = MasterPowerSwitch.getInstance();
            int count = power.logAccess();
            System.out.println(player + " accessed Master Power Switch. Total accesses so far: " + count);
        }
    }
}

```






## OUTPUT:



## RESULT:
The program successfully demonstrates the Singleton pattern by ensuring a single shared master power switch and maintaining a global access count across all player accesses.

