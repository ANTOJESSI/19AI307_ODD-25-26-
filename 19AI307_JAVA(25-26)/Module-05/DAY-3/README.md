# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Read a file and print only the lines containing the word "Java".

 
For example:

Input	Result
I love Java
Python is good
exit
Lines containing the word 'Java':
I love Java

## AIM:
To write a Java program that reads multiple lines of input and prints only the lines containing the word "Java".

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:



```
import java.util.ArrayList;
import java.util.Scanner;

public class PrintJavaLines {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        ArrayList<String> matchingLines = new ArrayList<>();

        String line;
        
        // Read input lines until "exit"
        while (!(line = sc.nextLine()).equals("exit")) {
            if (line.contains("Java")) {
                matchingLines.add(line);
            }
        }

        // Print results
        System.out.println("Lines containing the word 'Java':");
        for (String s : matchingLines) {
            System.out.println(s);
        }

        sc.close();
    }
}

```



## OUTPUT:



## RESULT:

The program successfully reads multiple lines and prints only the lines containing "Java".
