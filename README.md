# Java_Programms
## 1. Reverse a String
        String str = "Happy Coidng";
        String rev = " ";
        for (int i = str.length()-1; i >=0; i--){
            rev = rev + str.charAt(i);
        }
        System.out.println("Reverse String is:" + rev);

## 2. Palindrome 
        String str = "cac";
         String rev = "";
        for (int i = str.length()-1; i >=0; i--){
            rev = rev + str.charAt(i);
        }
        if(str.equals(rev)){
            System.out.println("Is Palindrome");
        }
        else
        {
            System.out.println("Not a Palindrome");
        }

## 3. Swap two numbers
         int a  = 10;
         int b = 20;
        int temp;
        temp = a;
        a = b;
        b = temp;
            System.out.println(a + " " + b);
        }
## 4. Even and Odd Number
          int num = 10;
               if(num % 2 == 0){
                   System.out.println("Even number");
               }else{
            System.out.println("Odd number");
               }
        
## 5. Prime Number Check
        int num = 29;
        boolean prime = true;
        for(int i = 2; i < num; i++){
            if(num % i == 0){
                prime = false;
                break;
            }
        }
            if(prime){
            System.out.println("Is Prime number");
        }else{
            System.out.println("Not a Prime Number");
        }
## 6. Right traingle Pattern (*******)
        int rows = 5;
        for(int i = 1; i <= rows; i++){
            for (int j = 1; j <= i; j++){
                System.out.print("* ");
            }
            System.out.println();
        }
## 7. Right Aligned Triangle (Left triangle)
            int rows = 5;
        for(int i = 1; i <= rows; i++){
            for(int j = i; j < rows; j++){
                System.out.print("  "); // Give the space two times
            }
            for(int j = 1; j <= i; j++){
                System.out.print("* ");
            }
            System.out.println();
        }
 
## 8. Right traingle (Number Pattern)
         int rows = 5;
        for(int i = 1; i <= rows; i++){
            for(int j = 1; j<=i; j++){
                System.out.print(j + " ");
            }
            System.out.println();
        }

## 9. Right Aligned Triangle(Number Pattern)
        int rows = 5;
        for(int i = 1; i <= rows; i++){
            for(int j = i; j<rows; j++){
                System.out.print("  ");
            }
            for(int j = 1; j <= i; j++){
                System.out.print(j+ " ");
            }
            System.out.println();
        }

## 10. Inverted Right Triangle (Reverse)
       int rows = 5;
        for(int i = rows; i >= 1; i--){
            for(int j = 1; j <= i; j++){
                System.out.print("* ");
            }
            System.out.println();
        }

## 11. Reverse Right Triangle(Number)
            int rows = 5;
        for(int i = rows; i >= 1; i--){
            for(int j = 1; j <= i; j++){
                System.out.print(j + " ");
            }
            System.out.println();
        }

## 12. Inverted Right Aligned Traingle
           int rows = 5;
        for(int i = rows; i>=1; i--){
            for(int j = i; j < rows; j++){
                System.out.print("  ");
            }
            for(int j = 1; j<=i; j++){
                System.out.print("* ");
            }
            System.out.println();
        }

## 13. Inverted Right Aligned triangle (Number Pattern)
            int rows = 5;
        for(int i = rows; i>=1; i--){
            for(int j = i; j < rows; j++){
                System.out.print("  ");
            }
            for(int j = 1; j<=i; j++){
                System.out.print(j + " ");
            }
            System.out.println();
        }
    

