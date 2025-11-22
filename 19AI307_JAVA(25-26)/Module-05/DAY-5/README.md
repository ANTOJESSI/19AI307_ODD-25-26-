# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Write a java program for determine the priority and name of the current thread.

Note : Read the threadname from the User

For example:

Input	Result
NewThread
Priority of Thread: 5
Name of Thread: NewThread
Thread[NewThread,5,main]



## AIM:
To write a Java program that reads a thread name from the user and displays the current thread’s name and priority

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input.
4.	Read the thread name from the user.
5.	Get the current thread using Thread.currentThread().
6.	Set the thread’s name using setName().
7.	Display the thread’s priority using getPriority().
8.	Display the thread’s name using getName().
9.	Display the thread’s details using toString().





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: ANTO JESSI A
RegisterNumber:  212222040009
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

public class ThreadInfo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Read thread name from user
        String threadName = sc.nextLine();

        // Get the current thread
        Thread current = Thread.currentThread();

        // Set the thread name
        current.setName(threadName);

        // Display results
        System.out.println("Priority of Thread: " + current.getPriority());
        System.out.println("Name of Thread: " + current.getName());
        System.out.println(current.toString());

        sc.close();
    }
}
```





## OUTPUT:

<img width="909" height="416" alt="image" src="https://github.com/user-attachments/assets/754dcdfe-e57b-4b20-ba45-cff2f8c0d609" />


## RESULT:
The program successfully sets the name of the current thread, and prints the thread’s priority, name, and details.
