# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:

Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.
## AIM:
To write a Java program that demonstrates the use of access specifiers, specifically using private for data hiding and public methods to access and modify values.

## ALGORITHM :
Start the program.

Import the necessary package 'java.util'

Create a class BankAccount with private variables accountNumber and balance.

Provide public getter and setter methods for both variables.

Inside the main method, create an object of BankAccount.

Use setter methods to assign values to accountNumber and balance.

Display the values using getter methods.

Stop the program.	





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Praveen K
RegisterNumber:  212223040152
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main 
{
    static class BankAccount 
    {
        private String accountNumber;
        private double balance;
        public String getAccountNumber()
        {
            return accountNumber;
        }
        public void setAccountNumber(String accountNumber) 
        {
            this.accountNumber = accountNumber;
        }
        public double getBalance() 
        {
            return balance;
        }
        public void setBalance(double balance)
        {
            this.balance = balance;
        }
    }

    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        BankAccount account = new BankAccount();
        String accNo = sc.nextLine();
        double bal = sc.nextDouble();
        account.setAccountNumber(accNo);
        account.setBalance(bal);
        System.out.println("Account Number: "+account.getAccountNumber());
        System.out.println("Balance: "+account.getBalance());
    }
}
```






## OUTPUT:
<img width="784" height="381" alt="image" src="https://github.com/user-attachments/assets/7b84cb3b-20f8-44fb-8718-798cc34514ee" />



## RESULT:
Thus, a Java program to implement Access Specifiers using private variables with public getter and setter methods was executed successfully.
