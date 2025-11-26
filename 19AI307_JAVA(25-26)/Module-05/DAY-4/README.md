# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a java program for determine the priority and name of the current thread.

Note : Read the threadname from the User

For example:

<img width="452" height="173" alt="image" src="https://github.com/user-attachments/assets/b804ea94-d472-424e-846c-7d5c56dad26d" />




## AIM:
To write a Java program that reads a thread name from the user and displays the current thread’s name and priority.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the thread name from the user.
4.	Get the current thread using Thread.currentThread().
5.	Set the thread’s name using setName().
6.	Display the thread’s priority using getPriority().
7.	Display the thread’s name using getName().
8.	Display the thread’s details using toString().
9.	Stop the program.



## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
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

<img width="878" height="487" alt="image" src="https://github.com/user-attachments/assets/77faf07c-c60d-43f9-9d80-6cdaf0b4e8de" />


## RESULT:

The program successfully sets the name of the current thread and prints its priority, name, and details.

