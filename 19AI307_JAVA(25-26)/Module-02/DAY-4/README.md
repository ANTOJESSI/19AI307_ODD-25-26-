# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Demonstrate variable shadowing by declaring an instance variable and a local variable with the same name inside a method. Print both values.
<img width="655" height="200" alt="image" src="https://github.com/user-attachments/assets/bff65272-d330-4a94-823b-3d3323c4eb79" />


## AIM:
To demonstrate variable shadowing by showing the difference between a local variable and an instance variable with the same name.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'.
3.	Declare an instance variable number.
4.	Create a method that takes a parameter with the same name number.
5.	Inside the method, print the local variable (number) and instance variable (this.number).
6.	In the main method, read input from the user.
7.	Create an object of the class and call the method, passing the input.
8.	Stop the program.




## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: ANTO JESSI A
RegisterNumber:  212222040009
*/
```

## SOURCE CODE:


```
import java.util.Scanner;

public class VariableShadowingExample {

    // Instance variable
    int number = 10;

    
    public void shadowVariable(int number) {
        // Local variable with the same name as the instance variable
        System.out.println("Local variable number: " + number);  // Refers to the method parameter
        System.out.println("Instance variable number: " + this.number);  // Refers to the instance variable
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int inputNumber = scanner.nextInt();

        VariableShadowingExample example = new VariableShadowingExample();
        example.shadowVariable(inputNumber);  

        scanner.close();
    }
}


```

## OUTPUT:

<img width="857" height="469" alt="image" src="https://github.com/user-attachments/assets/184f6340-39fe-4121-b55c-fb06dbb4e49f" />


## RESULT:
The program successfully demonstrates variable shadowing by printing both local and instance variable values.
