# Ex11 Convert HashSet to ArrayList in Java

## DATE: 20/09/2026

## AIM:

To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.

## Algorithm

1. Create a `HashSet` and read distinct integer elements into it.
2. Create an `ArrayList` using the elements of the `HashSet`.
3. Store all HashSet elements in the ArrayList.
4. Traverse the ArrayList using a loop.
5. Display the elements of the ArrayList.

## Program:

```java
/*
Program to convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: LAKSHMIDHAR N
RegisterNumber:  212224230138
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();

        for (int i = 0; i < n; i++) {
            set.add(sc.nextInt());
        }

        ArrayList<Integer> list = new ArrayList<>(set);

        for (int num : list) {
            System.out.print(num + " ");
        }
    }
}
```

## Output:

<img width="380" height="140" alt="image" src="https://github.com/user-attachments/assets/ea7e21bd-278b-491d-bd8c-74f6d43e7ac2" />


## Result:

The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList.
