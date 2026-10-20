```markdown
# Java Method Overloading Examples

This project demonstrates **method overloading** in Java through two examples:

1. Calculating the area of a square and rectangle  
2. Multiplying two or three integers  

Method overloading allows multiple methods in the same class to share the same name, as long as their parameter lists differ.

## Example 1: Area Calculation

The `main1` class contains two overloaded `area` methods:

| Method | Parameters | Purpose | Example |
|---|---:|---|---|
| `area(int side)` | 1 | Calculates the area of a square | `area(3)` returns `9` |
| `area(int length, int width)` | 2 | Calculates the area of a rectangle | `area(3, 5)` returns `15` |

### Source Code

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

### Expected Output

```text
9
15
```

## Example 2: Multiplication

The `multiply` class contains two overloaded `multiply` methods:

| Method | Parameters | Purpose | Example |
|---|---:|---|---|
| `multiply(int a, int b)` | 2 | Multiplies two integers | `multiply(7, 2)` returns `14` |
| `multiply(int a, int b, int c)` | 3 | Multiplies three integers | `multiply(1, 2, 9)` returns `18` |

### Source Code

```java
package inheritance;

public class multiply {
    int multiply(int a, int b) {
        return a * b;
    }

    int multiply(int a, int b, int c) {
        return a * b * c;
    }
}

class main {
    public static void main(String[] args) {
        multiply obj = new multiply();
        System.out.println(obj.multiply(7, 2));
        System.out.println(obj.multiply(1, 2, 9));
    }
}
```

### Expected Output

```text
14
18
```

## How to Run

### Example 1

1. Save the code in a file named `main.java`.
2. Compile the program:

```bash
javac main.java
```

3. Run the program:

```bash
java main
```

### Example 2

1. Save the code in a file named `multiply.java` inside a folder named `inheritance`.
2. From the parent directory of `inheritance`, compile the program:

```bash
javac inheritance/multiply.java
```

3. Run the program:

```bash
java inheritance.main
```

## Key Concept

**Method overloading** improves code readability by allowing related methods to use the same name with different parameter lists. Java selects the appropriate method at compile time based on the number and types of arguments passed.
```
