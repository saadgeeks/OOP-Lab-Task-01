# Java Method Overloading Example

This project demonstrates **method overloading** in Java. The `main1` class defines two methods with the same name, `area`, but different parameter lists.

## Overview

The program calculates the area of a square and a rectangle using overloaded methods. Java determines which method to call based on the number and types of arguments provided.

## Method Details

| Method | Parameters | Purpose | Example |
|---|---:|---|---|
| `area(int side)` | 1 | Calculates the area of a square | `area(3)` returns `9` |
| `area(int length, int width)` | 2 | Calculates the area of a rectangle | `area(3, 5)` returns `15` |

## Source Code

```java
class main1 {
    int area(int side) {
        return side * side;
    }

    int area(int length, int width) {
        return length * width;
    }
}

class main {
    public static void main(String[] args) {
        main1 obj = new main1();
        System.out.println(obj.area(3));
        System.out.println(obj.area(3, 5));
    }
}
```

## Expected Output

```text
9
15
```

## How to Run

1. Save the source code in a file named `main.java`.
2. Compile the program:

```bash
javac main.java
```

3. Run the compiled program:

```bash
java main
```

## Key Concept

**Method overloading** allows multiple methods within the same class to have the same name, provided their parameter lists differ. In this example, one method accepts a single side length for a square, while the other accepts a length and width for a rectangle.
