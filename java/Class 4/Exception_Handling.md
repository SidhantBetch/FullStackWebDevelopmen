# Exception Handling
Exception Handling in Java is a mechanism used to handle runtime errors so that the program does not terminate abruptly and the normal flow of the program can continue. ⚠️

## What is an Exception?
An exception is an unexpected event that occurs during program execution and disrupts the normal flow of the program.

Examples
- Dividing a number by zero
- Accessing an invalid array index
- Opening a file that does not exist

Example:
    
    int a = 10;
    int b = 0;
    int c = a / b;   // ArithmeticException

### Types of Exceptions in Java
#### 1️⃣ Checked Exceptions
Checked at compile time.  
Must be handled using try-catch or throws.  

Examples:
- IOException
- SQLException
- FileNotFoundException

#### 2️⃣ Unchecked Exceptions
Occur at runtime.  
Not checked during compilation.

Examples:
- ArithmeticException
- NullPointerException
- ArrayIndexOutOfBoundsException
  
-----------------------------------------------------------------------------------------------------------------------------

## Exception Handling Keywords
Java provides five keywords for exception handling.

| Keyword	| Description |
|---------|-------------|
try	|Contains code that may cause an exception
catch	|Handles the exception
finally	|Executes always (optional)
throw	|Used to throw an exception manually
throws	|Declares exceptions

### 1️⃣ try-catch Example
    public class Test {
        public static void main(String[] args) {
    
            try {
                int a = 10;
                int b = 0;
                int c = a / b;
            }
            catch (ArithmeticException e) {
                System.out.println("Cannot divide by zero");
            }
    
            System.out.println("Program continues");
        }
    }


Output:

    Cannot divide by zero
    Program continues

### 2️⃣ try-catch-finally
The finally block always executes whether an exception occurs or not.

Example:

    try {
        int num = 10 / 0;
    }
    catch (ArithmeticException e) {
        System.out.println("Error occurred");
    }
    finally {
        System.out.println("This block always executes");
    }

### 3️⃣ throw Keyword
Used to explicitly throw an exception.

Example:

    throw new ArithmeticException("Error occurred");

### 4️⃣ throws Keyword
Used to declare exceptions in method definition.

Example:

    void readFile() throws IOException {
    }
