# Method in Java
A method in Java is a block of code that performs a specific task.
It runs only when it is called. 🔹
Methods help make programs organized, reusable, and easier to understand.

Syntax of a Method

    returnType methodName(parameters) {
        // method body
    }


Example parts:
- *returnType* → type of value returned (int, void, String, etc.)
- *methodName* → name of the method
- *parameters* → input values
- *method body* → code that performs the task

Example Program

    class Student {
    
        void display() {
            System.out.println("Hello Java");
        }
    
        public static void main(String[] args) {
            Student s = new Student();
            s.display();   // calling the method
        }
    }


Output

    Hello Java
    

## Types of Methods

### 1️⃣ Method without parameters
    void show() {
        System.out.println("Welcome");
    }


### 2️⃣ Method with parameters
    void add(int a, int b) {
        int sum = a + b;
        System.out.println(sum);
    }


### 3️⃣ Method with return value
    int add(int a, int b) {
        return a + b;
    }

## Example with Return Value
    class Test {
    
        int add(int a, int b) {
            return a + b;
        }
    
        public static void main(String[] args) {
            Test t = new Test();
            int result = t.add(5, 3);
            System.out.println(result);
        }
    }


### Output
    8
