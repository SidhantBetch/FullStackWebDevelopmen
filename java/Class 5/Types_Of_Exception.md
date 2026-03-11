# In Java, Exceptions are mainly divided into two types:

1️⃣ Checked Exceptions  
2️⃣ Unchecked Exceptions  
Both are part of the Exception Handling mechanism. ⚠️

-------------------------------------------------------------------------------------------------------------

## 1️⃣ Checked Exceptions
Checked exceptions are checked at compile time by the Java compiler.
The programmer must handle them using try-catch or throws.

Examples
- IOException
- SQLException
- FileNotFoundException
- ClassNotFoundException

Example Code

    import java.io.FileReader;
    
    public class Test {
        public static void main(String[] args) {
            try {
                FileReader file = new FileReader("test.txt");
            }
            catch (Exception e) {
                System.out.println("File not found");
            }
        }
    }
Here the compiler forces us to handle the exception.

-------------------------------------------------------------------------------------------------------------

## 2️⃣ Unchecked Exceptions
Unchecked exceptions occur during runtime and are not checked by the compiler.  
They usually happen because of programming mistakes.

Examples
- ArithmeticException
- NullPointerException
- ArrayIndexOutOfBoundsException
- NumberFormatException

Example Code

    public class Test {
        public static void main(String[] args) {
            int a = 10;
            int b = 0;
    
            int c = a / b;  // ArithmeticException
        }
    }

-------------------------------------------------------------------------------------------------------------

## Exception Hierarchy (Simple)
```
 Throwable
   │
   ├── Exception
   │     ├── Checked Exceptions
   │     └── RuntimeException (Unchecked)
   │
   └── Error 
```

-------------------------------------------------------------------------------------------------------------

## Difference Between Checked and Unchecked Exceptions
|Feature	|Checked Exception	|Unchecked Exception|
|---------|-------------------|-------------------|
Checked by compiler|	Yes	|No
Occurs at	Compile |time	|Runtime
Handling required	|Mandatory	|Optional
Example	|IOException	|ArithmeticException
