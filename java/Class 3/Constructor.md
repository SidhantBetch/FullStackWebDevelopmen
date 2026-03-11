# Constructor in Java
A constructor in Java is a special method that is used to initialize an object when the object is created. 

When you create an object of a class, the constructor is automatically called.



## Key Points
The constructor name must be the same as the class name.

A constructor does not have a return type (not even void).

It is called automatically when an object is created.

It is mainly used to initialize variables.



## Example
    class Student {
    
        int id;
        String name;
    
        // Constructor
        Student() {
            id = 1;
            name = "Kimi";
        }
    
        void display() {
            System.out.println(id + " " + name);
        }
    
        public static void main(String[] args) {
            Student s1 = new Student();   // Constructor is called here
            s1.display();
        }
    }

Output

    1 Kimi




## Types of Constructors

### 1️⃣ Default Constructor
A constructor with no parameters.

    Student() {
        System.out.println("Default constructor");
    }


### 2️⃣ Parameterized Constructor
A constructor that accepts parameters.

    Student(int i, String n) {
        id = i;
        name = n;
    }

### Example of Parameterized Constructor
    class Student {
    
        int id;
        String name;
    
        Student(int i, String n) {
            id = i;
            name = n;
        }
    
        void display() {
            System.out.println(id + " " + name);
        }
    
        public static void main(String[] args) {
            Student s1 = new Student(101, "Rahul");
            s1.display();
        }
    }
