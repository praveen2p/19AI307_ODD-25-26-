# Ex.No:3(F) WRAPPER CLASS

## QUESTION:

Find the largest digit in a number using wrapper class methods.
## AIM:
To write a Java program to find the largest digit in a given number using Wrapper Class methods.

## ALGORITHM :
```
Start the program.
Import the necessary package 'java.util'
Read the number from the user.
Convert the number to a string using wrapper class Integer.toString().
Traverse each character, convert it back to an integer using Character.getNumericValue().
Compare digits and store the largest digit.
Display the largest digit.
Stop the program.
```




## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Praveen K
RegisterNumber:  212223040152
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine(); 

        int largest = 0;

        for (int i = 0; i < input.length(); i++) 
        {
            int digit = Character.getNumericValue(input.charAt(i));
            if (digit > largest) {
                largest = digit;
            }
        }

        System.out.println("The largest digit is: " + largest);
        sc.close();
    }
}
```





## OUTPUT:

<img width="630" height="247" alt="image" src="https://github.com/user-attachments/assets/030d9aba-9e13-475c-abbb-af621297534f" />


## RESULT:
Thus, the program to find the largest digit in a number using Wrapper Class methods was successfully executed.
