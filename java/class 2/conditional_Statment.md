# Conditional Statment
A conditional statement is used to make decisions in a program.
It executes different blocks of code depending on whether a condition is true or false.

  
## Types of Conditional Statements in Java
  ### 1️⃣ if Statement
  Executes a block of code only if the condition is true.
        
 #### Example
      class Test {
          public static void main(String[] args) {
              int age = 20;
      
              if(age >= 18){
                  System.out.println("You can vote");
              }
          }
      }
    
  ### 2️⃣ if-else Statement
  Used when there are two possible conditions.
        
  #### Example
        class Test {
            public static void main(String[] args) {
                int number = 10;
        
                if(number % 2 == 0){
                    System.out.println("Even number");
                }
                else{
                    System.out.println("Odd number");
                }
            }
        }
    
  ### 3️⃣ if-else if-else Statement
  Used when there are multiple conditions.
        
  #### Example
        class Test {
            public static void main(String[] args) {
                int marks = 75;
        
                if(marks >= 90){
                    System.out.println("Grade A");
                }
                else if(marks >= 60){
                    System.out.println("Grade B");
                }
                else{
                    System.out.println("Grade C");
                }
            }
        }
    
  ### 4️⃣ switch Statement
  Used when there are many possible values of a variable.
        
  #### Example
        class Test {
            public static void main(String[] args) {
                int day = 2;
        
                switch(day){
                    case 1:
                        System.out.println("Monday");
                        break;
        
                    case 2:
                        System.out.println("Tuesday");
                        break;
        
                    default:
                        System.out.println("Invalid day");
                }
            }
        }
