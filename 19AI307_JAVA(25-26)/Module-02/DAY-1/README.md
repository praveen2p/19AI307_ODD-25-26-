# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:

Create a class Person with attributes name and age. Write a method greet() that prints: Hello, my name is and I am years ol.
## AIM:
To write a Java program that demonstrates the concept of Class and Object using a Person class with attributes and a method.

## ALGORITHM :
Start the program.

Import the necessary package 'java.util'

Create a class named Person with attributes name and age.

Define a method greet() that prints the message using the attributes.

In the main() method, create an object of the Person class.

Read the name and age values from the user.

Call the greet() method using the object.

End the program.	





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Praveen K
RegisterNumber:  212223040152
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class prog {
    String name;
    int age;

    prog(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void greet() 
    {
        System.out.println("Hello, my name is " + name + " and I am " + age + " years old.");
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
       
        String name = scanner.nextLine(); 
        int age = scanner.nextInt();      

        prog person = new prog(name, age); 
        person.greet(); 

    }


}

```






## OUTPUT:
<img width="1165" height="305" alt="image" src="https://github.com/user-attachments/assets/26521b1a-1e82-4650-b9b7-1ebd00d7d9e1" />



## RESULT:
Thus, the Java program to implement a Class and Object using a Person class was successfully executed and verified.
