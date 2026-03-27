# Ex.No:3(E) INNER CLASS

## QUESTION:

Write a Java program to create an inner class and access it from the outer class.
## AIM:
To write a Java program that demonstrates the use of an Inner Class and how it can be accessed from the Outer Class

## ALGORITHM :
```
Start the program.
Import the necessary package 'java.util'
Create an outer class.
Inside the outer class, declare and define an inner class.
Create an object of the outer class.
Using the outer class object, create an object of the inner class.
Call a method of the inner class through its object.
Display the output.
Stop the program.
```






## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Praveen K
RegisterNumber: 212223040152
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

public class OuterClass 
{
    class InnerClass
    {
        void displayMessage(String name)
        {
            System.out.println("Hello, " + name + "! This message is from the Inner Class.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        OuterClass outer = new OuterClass();          
        OuterClass.InnerClass inner = outer.new InnerClass(); 
        inner.displayMessage(name); 
    }
}
```





## OUTPUT:
<img width="1129" height="248" alt="image" src="https://github.com/user-attachments/assets/cb991414-754a-4a4e-9466-610dcdd1934e" />



## RESULT:
Thus, the Java program to implement an Inner Class and access it from the Outer Class was successfully executed.
