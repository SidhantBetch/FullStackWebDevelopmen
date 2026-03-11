# Class
A class is a blueprint or template used to create objects.
It defines variables (data) and methods (functions).

Example:

    class Student {
        int id;
        String name;
    
        void display() {
            System.out.println(id + " " + name);
        }
    }
  
Here:
- `Student` → Class
- `id and name` → Variables 
- `display()` → Method

# Object
An object is an instance of a class.
It represents a real-world entity and can access the class variables and methods.

Example:

    class Student {
        int id;
        String name;
    
        void display() {
            System.out.println(id + " " + name);
        }
    
        public static void main(String[] args) {
            Student s1 = new Student();   // object creation
    
            s1.id = 101;
            s1.name = "Rahul";
    
            s1.display();
        }
    }
Here:
- `s1` → Object of class `Student`
