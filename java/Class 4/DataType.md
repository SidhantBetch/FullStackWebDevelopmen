# Data Types in Java
In Java data types are divided into two main categories:

1️⃣ Primitive Data Types  
2️⃣ Non-Primitive Data Types  

## 1️⃣ Primitive Data Types
Primitive data types are basic built-in data types provided by Java.

### Java has 8 primitive data types.

| Data Type	| Size	  | Example	      | Description  |
|-----------|---------|---------------|--------------|
|byte	      |1 byte	  |byte a = 10;	  |Small integer |
|short	    |2 bytes	|short b = 200;	|Small integer |
|int	      |4 bytes	|int c = 1000;	|Most used integer |
|long	      |8 bytes	|long d = 100000L;	|Large integer |
|float	    |4 bytes	|float e = 5.5f;	  |Decimal number |
|double	    |8 bytes	|double f = 10.55;	|Large decimal |
|char	      |2 bytes	|char g = 'A';	    |Single character |
|boolean	  |1 bit	  |boolean h = true;	|True or False |

Example Program

    public class DataTypeExample {
        public static void main(String[] args) {
    
            int number = 10;
            float price = 12.5f;
            char grade = 'A';
            boolean status = true;
    
            System.out.println(number);
            System.out.println(price);
            System.out.println(grade);
            System.out.println(status);
        }
    }

### 2️⃣ Non-Primitive Data Types
Non-primitive data types are reference types that store addresses of objects.

Examples:

- String
- Array
- Class
- Object
- Interface

Example:

    String name = "Kimi";

## Difference Between Primitive and Non-Primitive
| Primitive	| Non-Primitive |
|-----------|---------------|
|Stores actual value	|Stores reference (address) |
|Built-in data types	|Created by programmer |
|Fixed size	|Size depends on object |
|Example: int, float	|Example: String, Array |
