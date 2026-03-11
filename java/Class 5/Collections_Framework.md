# Collections Framework
The Collections Framework in Java is a set of classes and interfaces that provide a standard way to store, manage, and manipulate groups of objects.  
It is part of the java.util package.  
Collections help perform operations like:  
- Storing data
- Searching
- Sorting
- Inserting
- Deleting elements

____________________________________________________________________________________________________________________________________________________________________

### 1️⃣ Main Interfaces of Collection Framework
The Collection Framework hierarchy is based on interfaces.
```mathematica
Iterable
   │
Collection
   │
 ┌───────┬────────┐
 List    Set      Queue
```
Another important interface is:

``` javascript
    Map
```

(Map is not a part of Collection but is included in the framework.)



### 2️⃣ List Interface
A List stores elements in ordered form and allows duplicates.  

- Common Classes:
- ArrayList
- LinkedList
- Vector

Example:
    
    import java.util.ArrayList;
    
    public class Test {
        public static void main(String[] args) {
            ArrayList<String> list = new ArrayList<>();
    
            list.add("Java");
            list.add("C++");
            list.add("Python");
    
            System.out.println(list);
        }
    }


Output:

    [Java, C++, Python]


Features:
- Maintains order
- Allows duplicate values



### 3️⃣ Set Interface
A Set stores unique elements (no duplicates).

Common Classes:
- HashSet
- LinkedHashSet
- TreeSet

Example:

    import java.util.HashSet;
    
    HashSet<Integer> set = new HashSet<>();
    set.add(10);
    set.add(20);
    set.add(10);
    
    System.out.println(set);


Output:

    [10, 20]


Features:
- No duplicate elements
- No guaranteed order (HashSet)



### 4️⃣ Queue Interface
Queue follows FIFO (First In First Out).

Common Classes:
- PriorityQueue
- ArrayDeque

Example:

    import java.util.PriorityQueue;
    
    PriorityQueue<Integer> q = new PriorityQueue<>();
    
    q.add(10);
    q.add(20);
    q.add(30);
    
    System.out.println(q);


    

### 5️⃣ Map Interface
A Map stores data in key-value pairs.

Common Classes:
- HashMap
- LinkedHashMap
- TreeMap

Example:

    import java.util.HashMap;
    
    HashMap<Integer,String> map = new HashMap<>();
    
    map.put(1,"Java");
    map.put(2,"Python");
    
    System.out.println(map);


Output:

    {1=Java, 2=Python}



### 6️⃣ Advantages of Collection Framework
Reduces programming effort  
Provides reusable data structures  
Improves performance  
Easy data manipulation  

_________________________________________________________________________________________________________________________________________________________________


## Main Classes of Collection Framework



### 1️⃣ ArrayList
Implements List interface  
Stores elements in dynamic array  
Allows duplicate elements  
Maintains insertion order  

Example:

    import java.util.ArrayList;
    
    ArrayList<String> list = new ArrayList<>();
    list.add("Java");
    list.add("C++");
    list.add("Python");
    
    System.out.println(list);


    

### 2️⃣ LinkedList
Implements List and Queue interfaces  
Uses linked list structure  
Allows duplicate elements  

Example:

    import java.util.LinkedList;
    
    LinkedList<Integer> list = new LinkedList<>();
    
    list.add(10);
    list.add(20);
    
    System.out.println(list);




### 3️⃣ Vector
Similar to ArrayList  
Synchronized (thread-safe)  
Allows duplicate elements  

Example:

    import java.util.Vector;
    
    Vector<String> v = new Vector<>();
    
    v.add("Apple");
    v.add("Mango");
    
    System.out.println(v);




### 4️⃣ HashSet
Implements Set interface  
Does not allow duplicate elements  
Does not maintain order  

Example:

    import java.util.HashSet;
    
    HashSet<Integer> set = new HashSet<>();
    
    set.add(10);
    set.add(20);
    set.add(10);
    
    System.out.println(set);


    

### 5️⃣ TreeSet
Implements Set interface  
Stores elements in sorted order  
Does not allow duplicates  

Example:

    import java.util.TreeSet;
    
    TreeSet<Integer> set = new TreeSet<>();
    
    set.add(30);
    set.add(10);
    set.add(20);
    
    System.out.println(set);


    

### 6️⃣ HashMap
Implements Map interface  
Stores data in key-value pairs  
Allows one null key  

Example:

    import java.util.HashMap;
    
    HashMap<Integer,String> map = new HashMap<>();
    
    map.put(1,"Java");
    map.put(2,"Python");
    
    System.out.println(map);
