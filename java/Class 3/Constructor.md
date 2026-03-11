# Constructor in Java
A constructor in Java is a special method that is used to initialize an object when the object is created.  
When you create an object of a class, the constructor is automatically called.



## Key Points
- The constructor name must be the same as the class name.  
- A constructor does not have a return type (not even void).  
- It is called automatically when an object is created.  
- It is mainly used to initialize variables.  



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

### 1️⃣ Non-Parameterized Constructor
A non-parameterized constructor is a constructor that does not take any parameters.  
It initializes the object with default or fixed values. 🧩

Syntax

    class ClassName {
    
        ClassName() {
            // constructor body
        }
    
    }

Example Program

    class Student {
    
        int id;
        String name;
    
        // Non-parameterized constructor
        Student() {
            id = 100;
            name = "Kimi";
        }
    
        void display() {
            System.out.println(id + " " + name);
        }
    
        public static void main(String[] args) {
            Student s1 = new Student();   // constructor called
            s1.display();
        }
    }



### 2️⃣ Parameterized Constructor
A parameterized constructor is a constructor that accepts parameters (arguments).  
It is used to initialize an object with specific values when the object is created.  

Syntax
class ClassName {

    ClassName(type parameter1, type parameter2) {
        // constructor body
    }

}

### Example
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
