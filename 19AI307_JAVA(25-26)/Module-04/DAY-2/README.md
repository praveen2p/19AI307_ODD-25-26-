# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:
In a large office, multiple departments send print jobs to a shared central printer. To manage load and prevent collision, a Print Spooler Manager handles all job submissions.

The IT team insists that there should be only one spooler manager instance in the entire system. Regardless of how many jobs or departments exist, all jobs must pass through this one manager.

Your task is to simulate a singleton print job queue. Each print job submitted increases the queue count.

## AIM:
To write a Java program that demonstrates the Singleton Design Pattern, ensuring only one instance of a Print Spooler Manager exists to handle job queue management.

## ALGORITHM :
```
Start the program.

Import the necessary package 'java.util'

Create a PrintSpooler class with:

A private static instance.

A private constructor.

A public static getInstance() method to return the single instance.

Maintain a counter that represents the number of print jobs.

In the main() method, simulate two departments submitting print jobs.

Access the same instance of the Print Spooler and increment the job count.

Display the print job queue.

Stop the program.
```




## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: Praveen K
RegisterNumber: 212223040152 
*/
```

## SOURCE CODE:

```
import java.util.*;

class PrintSpoolerManager {
    private static PrintSpoolerManager instance;
    private int jobCount = 0;

    private PrintSpoolerManager() {}

    public static PrintSpoolerManager getInstance() {
        if (instance == null) {
            instance = new PrintSpoolerManager();
        }
        return instance;
    }

    public int submitJob(String department) {
        jobCount++;
        return jobCount;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String dept = sc.nextLine();
            PrintSpoolerManager spooler = PrintSpoolerManager.getInstance();
            int total = spooler.submitJob(dept);
            System.out.println(dept + " submitted a print job. Total Jobs in Queue: " + total);
        }
    }
}
```





## OUTPUT:
<img width="1190" height="434" alt="image" src="https://github.com/user-attachments/assets/8e124f46-bd4f-40eb-880c-219e1cdfec36" />



## RESULT:
Thus, the program to simulate a Singleton Print Spooler Manager using SOLID principles was successfully implemented and executed.
