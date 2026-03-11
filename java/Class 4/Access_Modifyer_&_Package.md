# Access Modifiers in Java
Access Modifiers define who can access a class, variable, method, or constructor.  

## Java has four types of access modifiers:
| Modifier	| Same Class	| Same Package	| Subclass	| Other Package |
|-----------|-------------|---------------|-----------|---------------|
|private	  |✅ Yes	    |❌ No	        |❌ No	    |❌ No         |
|default	  |✅ Yes	    |✅ Yes	      |❌ No  	  |❌ No         |
|protected	|✅ Yes	    |✅ Yes	      |✅ Yes	  |❌ No         |
|public	    |✅ Yes	    |✅ Yes	      |✅ Yes	  |✅ Yes        |


## 1. Private
Accessible only inside the same class.  
Used for data hiding.

Example:
    
    class Student {
        private int age;
    
        void setAge(int a) {
            age = a;
        }
    
        void showAge() {
            System.out.println(age);
        }
    }
Here, age cannot be accessed outside the class.

## 2. Default (No Modifier)
When no modifier is written, it becomes default.  
Accessible only inside the same package.

Example:
    
    class Test {
        int number = 10;
    }
    
## 3. Protected
Accessible within the same package and in subclasses (child classes).  

Example:

    class Animal {
        protected void eat() {
            System.out.println("Animal eats food");
        }
    }

## 4. Public
Accessible from anywhere in the program.

Example:

    public class Hello {
        public void display() {
            System.out.println("Hello Java");
        }
    }


----------------------------------------------------------------------------------------------------------------------------------
# Package in Java
A package is a group of related classes and interfaces.  
It helps organize large programs and avoid name conflicts.

Example:

    java.util
    java.lang
    java.io

## Types of Packages
### 1. Built-in Packages
These are already provided by Java.

Examples:

- java.util → utility classes (ArrayList, Scanner)
- java.lang → basic classes (String, Math)
- java.io → input/output classes

Example:

    import java.util.Scanner;
    
    class Test {
        public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
        }
    }

## 2. User-defined Packages
Programmers can create their own packages.

Example:

    package mypackage;
    
    public class Test {
        public void show() {
            System.out.println("This is my package");
        }
    }

### Creating a Package

Syntax:
    
    package package_name;
    
Example:

    package com.company;
