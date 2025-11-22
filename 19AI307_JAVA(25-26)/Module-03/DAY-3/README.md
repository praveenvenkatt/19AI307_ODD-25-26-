# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create abstract class BankAccount with method calculateInterest(). Extend it in SavingsAccount and FixedDepositAccount.

Input Format:

First line: 1 for SavingsAccount, 2 for FixedDepositAccount
- If 1: next line → balance (double)
- If 2: next line → amount (double) and years (int)

Output Format:

- A single line showing interest earned rounded to 2 decimal places.


## AIM:
To write a Java program that uses abstraction by creating an abstract class BankAccount with an abstract method calculateInterest(), and implementing it in SavingsAccount and FixedDepositAccount to compute interest based on user input.

## ALGORITHM :
Step 1: Start the program.

Step 2: Create an abstract class BankAccount with an abstract method calculateInterest().

Step 3: Create a subclass SavingsAccount that extends BankAccount and calculates interest based on balance.

Step 4: Create another subclass FixedDepositAccount that calculates interest based on deposit amount and number of years.

Step 5: Read the user input to determine whether it is a savings or fixed deposit account.

Step 6: Create the appropriate account object and call the calculateInterest() method.

Step 7: Print the interest rounded to two decimal places and end the program.





## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: Praveen V
RegisterNumber:  212222040121
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

abstract class BankAccount 
{
    abstract double calculateInterest();
}

class SavingsAccount extends BankAccount 
{
    double balance;
    SavingsAccount(double balance) 
    {
        this.balance = balance;
    }
    @Override
    double calculateInterest() 
    {
        return balance * 0.04; 
    }
}

class FixedDepositAccount extends BankAccount 
{
    double amount;
    int years;
    FixedDepositAccount(double amount, int years) 
    {
        this.amount = amount;
        this.years = years;
    }
    @Override
    double calculateInterest() 
    {
        return amount * 0.07 * years; 
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int type = sc.nextInt();
        BankAccount acc;

        if (type == 1) 
        {
            double balance = sc.nextDouble();
            acc = new SavingsAccount(balance);
        } 
        else 
        {
            double amount = sc.nextDouble();
            int years = sc.nextInt();
            acc = new FixedDepositAccount(amount, years);
        }

        System.out.printf("%.2f%n", acc.calculateInterest());
    }
}

```






## OUTPUT:



## RESULT:
The program successfully calculates and prints the interest earned for either a SavingsAccount or FixedDepositAccount based on user input.

