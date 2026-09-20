# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()

## DATE: 20/09/2026

## AIM:

To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.

## Algorithm

1. Create an array with at least 10 elements.
2. Read the elements of the array from the user.
3. Use `Arrays.fill()` to fill the first 10 elements with the value `5`.
4. Traverse the array and display its elements.
5. Verify that the first 10 elements contain the constant value `5`.

## Program:

```java
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int[] arr = new int[10];

        Arrays.fill(arr, 5);

        for (int num : arr) {
            System.out.print(num + " ");
        }
    }
}
```

## Output:

<img width="395" height="65" alt="image" src="https://github.com/user-attachments/assets/e7eb10d6-5625-4613-8bef-210ba7e1ec41" />


## Result:

The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
