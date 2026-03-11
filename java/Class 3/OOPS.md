# 1️⃣ Encapsulation
Encapsulation means wrapping data and methods together in a single unit (class) and restricting direct access to data.  
It is implemented using private variables and public getter/setter methods.

## Example
    class Student {
        private int age;
    
        public void setAge(int a) {
            age = a;
        }
    
        public int getAge() {
            return age;
        }
    }


### Benefits:
- Data security 🔒
- Better control over data


# 2️⃣ Inheritance
Inheritance allows one class to acquire properties and methods of another class.  
The class that inherits is called child class, and the class being inherited is parent class.

## Example
    class Animal {
        void eat() {
            System.out.println("Animal eats");
        }
    }

    class Dog extends Animal {
        void bark() {
            System.out.println("Dog barks");
        }
    }


### Here:
- Animal → parent class
- Dog → child class

## Types of inheritance in Java:
1 Single inheritance  
2 Multilevel inheritance  
3 Hierarchical inheritance  



# 3️⃣ Polymorphism
Polymorphism means one name, many forms.

## Types of Polymorphism:
### 1. Compile-Time Polymorphism (Method Overloading)  
Same method name with different parameters.

Example:

    class MathOperation {
        int add(int a, int b) {
            return a + b;
        }
    
        int add(int a, int b, int c) {
            return a + b + c;
        }
    }

### 2. Run-Time Polymorphism (Method Overriding)
Child class redefines a method of parent class.

Example:

    class Animal {
        void sound() {
            System.out.println("Animal makes sound");
        }
    }
    
    class Dog extends Animal {
        void sound() {
            System.out.println("Dog barks");
        }
    }



# 4️⃣ Abstraction
Abstraction means hiding implementation details and showing only essential features.

## It is implemented using:
- Abstract classes
- Interfaces

Example (Abstract Class)

    abstract class Shape {
        abstract void draw();
    }
    
    class Circle extends Shape {
        void draw() {
            System.out.println("Drawing Circle");
        }
    }

Example (Interface)

    interface Animal {
        void sound();
    }
    
    class Dog implements Animal {
        public void sound() {
            System.out.println("Dog barks");
        }
    }
