# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Create a Java class Book with instance variables title and author.

## AIM:
To write a Java program to demonstrate variable scope and the use of a constructor to initialize instance variables.

## ALGORITHM :
	Start the program.
 
Import the necessary package 'java.util'

Create a class named Book with instance variables title and author.

Create a parameterized constructor to initialize these variables.

In the main() method, create an object of the Book class and pass values through the constructor.

Display the values.

End the program.





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Praveen K
RegisterNumber: 212223040152
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Book 
{
    String title;
    String author;
    Book(String t, String a)
    {
        title = t;
        author = a;
    }

    void display() {
        System.out.println("Book Title: " + title);
        System.out.println("Author: " + author);
    }
}

class prog {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        
        String title = sc.nextLine();   
        String author = sc.nextLine(); 

        Book b = new Book(title, author);
        b.display();

        sc.close();
    }
}
```






## OUTPUT:
<img width="792" height="315" alt="image" src="https://github.com/user-attachments/assets/831000af-1d27-469f-943d-f13cce139494" />



## RESULT:
Thus, the Java program to demonstrate variable scope and constructor was executed successfully.
