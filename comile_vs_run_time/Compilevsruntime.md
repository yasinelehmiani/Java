# **Difference Between Compile-Time and Run-Time**

## **1. Compile-Time**
Compile-time refers to the period **when the code is compiled** before execution. Errors that occur at this stage are called **compile-time errors** (e.g., syntax errors, type mismatches).  

### **Example of Compile-Time Errors in Java**
```java
public class CompileTimeExample {
    public static void main(String[] args) {
        int num = "Hello"; // ❌ Compile-time error: Type mismatch
        System.out.println(num);
    }
}
```
**Why does this fail?**  
- The compiler detects an error because `"Hello"` is a `String`, but `num` is an `int`.  
- The program **will not run** until this error is fixed.

---

## **2. Run-Time**  
Run-time refers to the period **when the program is running** after successful compilation. Errors that occur at this stage are called **run-time errors** (e.g., dividing by zero, accessing an invalid array index).  

### **Example of a Run-Time Error**  
```java
public class RunTimeExample {
    public static void main(String[] args) {
        int a = 10;
        int b = 0;
        System.out.println(a / b); // ❌ Run-time error: Division by zero
    }
}
```
**Why does this fail?**  
- The compiler does not detect any errors because the syntax is correct.
- However, at **runtime**, `10 / 0` causes an **ArithmeticException** (division by zero), and the program crashes.

---

## **Key Differences Between Compile-Time and Run-Time**
| Feature          | Compile-Time | Run-Time |
|-----------------|-------------|----------|
| **Definition**  | When the code is being compiled | When the program is running |
| **Errors**      | Syntax errors, type mismatches | Exceptions, logical errors |
| **Detection**   | Errors are caught before execution | Errors occur during execution |
| **Examples of Errors** | Missing semicolon, wrong variable type | Division by zero, accessing an invalid array index |
| **Resolution**  | Must be fixed before running the program | May cause program crashes if not handled |

---

## **Real-World Analogy**  
- **Compile-Time**: Checking a recipe before cooking (correcting missing ingredients, fixing steps).  
- **Run-Time**: Actually cooking the dish (if you make a mistake, like burning food, it happens while running the process).  

---

Let me know if you need further modifications! 🚀
