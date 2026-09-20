# Ex12 Add Elements from an Array into a TreeSet

## DATE: 20/09/2026

## AIM:

To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.

## Algorithm

1. Read the number of elements and store them in an array.
2. Create a `TreeSet` to store the elements.
3. Add each array element into the `TreeSet`.
4. The `TreeSet` automatically removes duplicates and stores elements in sorted order.
5. Display the elements of the `TreeSet`.

## Program:

```java
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> set = new TreeSet<>();

        for (int num : arr) {
            set.add(num);
        }

        for (int num : set) {
            System.out.print(num + " ");
        }
    }
}
```

## Output:

<img width="396" height="122" alt="image" src="https://github.com/user-attachments/assets/763a1017-22ff-4f94-8171-dbec9b2ab423" />


## Result:

The program successfully adds elements from an array into a TreeSet and displays the elements in sorted order.
 q
