# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
If an Integer object is set to null, and you attempt to call .toString() on it, what happens? How can you prevent your code from throwing an exception in such cases?



## AIM:
To write a Java program to demonstrate NullPointerException when calling .toString() on a null Integer object and to handle the exception using try-catch.

## ALGORITHM :
```
Start the program.
Import the necessary package 'java.util'
Read an integer value from the user.
Assign null if the user enters 0 (or a specific case).
Try to call .toString() method on the Integer object.
Catch the NullPointerException and display a meaningful message.
Display output and end the program.
```





## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Praveen K
RegisterNumber: 212223040152 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class NullCheck
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        Integer num = sc.nextInt(); 
        try 
        {
            if (num == 0) 
            {
                num = null;
            }
            System.out.println(num.toString());

        } 
        catch (NullPointerException e) 
        {
            System.out.println("Null Integer");
        }
    }
}
```






## OUTPUT:
<img width="474" height="290" alt="image" src="https://github.com/user-attachments/assets/fdd6ac58-bb96-4b73-bc08-be0d27b0b4ad" />



## RESULT:
Thus, the program demonstrates that calling .toString() on a null object causes a NullPointerException, and the exception can be prevented using a try-catch block.
