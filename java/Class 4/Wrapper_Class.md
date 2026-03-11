# Wrapper Class
Wrapper classes wrap primitive data types into an object form.  
This is useful because many Java features (like Collections, Generics) work only with objects, not primitive types.

## Primitive Data Type vs Wrapper Class
| Primitive Type	| Wrapper Class |
|-----------------|---------------|
|byte	|Byte
short	|Short
int	|Integer
long	|Long
float	|Float
double	|Double
char	|Character
boolean	|Boolean

Example

    public class WrapperExample {
        public static void main(String[] args) {
    
            int num = 10;          // primitive data type
            Integer obj = num;     // wrapper object (Autoboxing)
    
            System.out.println(obj);
        }
    }


Here:
- int → primitive type
- Integer → wrapper class

## Two Important Concepts
#### 1️⃣ Autoboxing
Automatic conversion of primitive type → wrapper object.

Example:

    int a = 5;
    Integer obj = a;

#### 2️⃣ Unboxing
Conversion of wrapper object → primitive type.

Example:

    Integer obj = 10;
    int a = obj;

## Example with ArrayList
Collections cannot store primitive types.  

❌ Wrong: 
    
    ArrayList<int> list = new ArrayList<>();  

✅ Correct:
    
    ArrayList<Integer> list = new ArrayList<>();  


**Because ArrayList works with objects only.**

## Advantages of Wrapper Classes
Used in Collections (ArrayList, LinkedList)  
Allows object representation of primitive data  
Provides utility methods  

Example:

    Integer num = Integer.parseInt("123");
