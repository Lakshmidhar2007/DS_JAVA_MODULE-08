# Ex15 Value Existence Check in a TreeMap

## DATE: 20/09/2026

## AIM:

To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm

1. Create a `TreeMap` and read key-value pairs from the user.
2. Store each key and its corresponding value in the `TreeMap`.
3. Read the value to be searched.
4. Use the `containsValue()` method to check whether the value exists in the `TreeMap`.
5. Display whether the specified value is present or not.

## Program:

```java
/*
Program to check whether a given value exists in a TreeMap.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        TreeMap<Integer, String> map = new TreeMap<>();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            String value = sc.next();
            map.put(key, value);
        }

        String searchValue = sc.next();

        if (map.containsValue(searchValue))
            System.out.println("Value exists");
        else
            System.out.println("Value does not exist");
    }
}
```

## Output:

<img width="397" height="227" alt="image" src="https://github.com/user-attachments/assets/97e41a49-ae5e-4834-a59e-9f8c79baeb00" />


## Result:

Thus, the program successfully checks whether a specified value exists in a TreeMap using the `containsValue()` method.
