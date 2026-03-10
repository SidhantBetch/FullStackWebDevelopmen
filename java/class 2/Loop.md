# Loop in Java
A loop is used to repeat a block of code multiple times until a condition becomes false.
Loops help avoid writing the same code again and again.


## Types of Loops in Java
### 1️⃣ for Loop
Used when the number of iterations is known.
        
#### Syntax
    for(initialization; condition; update){
        // code
    }
        
#### Example
    class Test {
        public static void main(String[] args) {
            for(int i = 1; i <= 5; i++){
                System.out.println(i);
            }
        }
    }
        
    
### 2️⃣ while Loop
Used when the number of iterations is not fixed.
        
#### Syntax
    while(condition){
        // code
    }
        
#### Example
    class Test {
        public static void main(String[] args) {
            int i = 1;
    
            while(i <= 5){
                System.out.println(i);
                i++;
            }
        }
    }
    
### 3️⃣ do-while Loop
This loop executes at least once, even if the condition is false.
        
#### Syntax
    do{
        // code
    }
    while(condition);

#### Example
    class Test {
        public static void main(String[] args) {
            int i = 1;
    
            do{
                System.out.println(i);
                i++;
            }
            while(i <= 5);
        }
    }
