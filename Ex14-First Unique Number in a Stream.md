# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap

## DATE: 20/09/2026

## AIM:

To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm

1. Read the number of elements and store the integers from the stream.
2. Create a `LinkedHashMap` to store each number and its frequency.
3. Traverse the stream and update the frequency of each number.
4. Traverse the `LinkedHashMap` in insertion order and find the first number with frequency one.
5. Display the first unique number.

## Program:

```java
/*
Program to track the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();

        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
        }

        int firstUnique = -1;

        for (int num : map.keySet()) {
            if (map.get(num) == 1) {
                firstUnique = num;
                break;
            }
        }

        if (firstUnique != -1)
            System.out.println(firstUnique);
        else
            System.out.println("No unique number");
    }
}
```

## Output:

<img width="390" height="145" alt="image" src="https://github.com/user-attachments/assets/56c7cc7f-1474-4549-9bf0-071c5a5bc3a0" />


## Result:

The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
