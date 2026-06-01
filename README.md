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

## 14. Decimal to Binary
        public class BinaryRepresentation {
            public static void main(String[] args) {

                int num    = 29;
                String binary = Integer.toBinaryString(num);  // Convert to binary
                int zeros  = 0;
                int ones   = 0;

                for (char c : binary.toCharArray()) {
                    if (c == '0') zeros++;
                    else          ones++;
                }

                System.out.println("Number      : " + num);
                System.out.println("Binary      : " + binary);
                System.out.println("Count of 0s : " + zeros);
                System.out.println("Count of 1s : " + ones);
            }
        }

## 15. Binary to Decimal
        public class BinaryToDecimal {
            public static void main(String[] args) {

                String binary  = "11101";
                int decimal    = Integer.parseInt(binary, 2);  // Convert binary to decimal
                System.out.println("Binary  : " + binary);
                System.out.println("Decimal : " + decimal);
            }
        }

## 16.Decimal to Octal
        public class DecimalToOctal {
            public static void main(String[] args) {

                int num      = 29;
                int n        = num;
                String octal = "";

                while (n > 0) {
                    octal = (n % 8) + octal;   // Get remainder and prepend
                    n    /= 8;
                }

                System.out.println("Decimal : " + num);
                System.out.println("Octal   : " + octal);
            }
        }

## 17. Octal to Decimal
        import java.util.Scanner;
        public class OctalToDecimal {
            public static void main(String[] args) {

                Scanner sc   = new Scanner(System.in);
                System.out.print("Enter an octal number: ");
                String octal = sc.next();
                int decimal  = Integer.parseInt(octal, 8);

                System.out.println("Octal   : " + octal);
                System.out.println("Decimal : " + decimal);
                sc.close();
            }
        }

## 18. Decimal to HexaDecimal
        public class DecimalToHexadecimal {
            public static void main(String[] args) {
                int num         = 255;
                String hex      = Integer.toHexString(num).toUpperCase();  // Convert to hex
                System.out.println("Decimal     : " + num);
                System.out.println("Hexadecimal : " + hex);
            }
        }

## 19. HexaDecimal to Decimal
        public class HexadecimalToDecimal {
            public static void main(String[] args) {
                String hex  = "FF";
                int decimal = Integer.parseInt(hex, 16);  // Convert hex to decimal
                System.out.println("Hexadecimal : " + hex);
                System.out.println("Decimal     : " + decimal);
                }
        }
## 20. Binary to Octal
        public class BinaryToOctal {
            public static void main(String[] args) {

                String binary = "11101";
                String octal  = Integer.toOctalString(Integer.parseInt(binary, 2));  
                System.out.println("Binary : " + binary);
                System.out.println("Octal  : " + octal);
            }
        }

## 21 .Octal to Binary
        public class OctalToBinary {
            public static void main(String[] args) {
                String octal  = "35";
                String binary = Integer.toBinaryString(Integer.parseInt(octal, 8)); 
                System.out.println("Octal  : " + octal);
                System.out.println("Binary : " + binary);
            }
        }

## 22 .Binary to HexaDecimal
        public class BinaryToHexadecimal {
            public static void main(String[] args) {

                String binary = "11101";
                String hex    = Integer.toHexString(Integer.parseInt(binary,                         2)).toUpperCase();  // Convert binary to hex

                System.out.println("Binary      : " + binary);
                System.out.println("Hexadecimal : " + hex);
                }
        }
## 23. Hexadecimal to Binary
        import java.util.Scanner;
        public class HexToBinary {
                public static void main(String[] args) {
                        Scanner sc = new Scanner(System.in);

                        System.out.print("Enter a hexadecimal number: ");
                        String hex = sc.nextLine();

                        int decimal = Integer.parseInt(hex, 16);
                        String binary = Integer.toBinaryString(decimal);

                        System.out.println("Binary equivalent: " + binary);

                        sc.close();
                        }
                }

## 24. Octal to Hexadecimal 
        import java.util.Scanner;

        public class OctalToHexadecimal {
            public static void main(String[] args) {
                Scanner sc = new Scanner(System.in);

                System.out.print("Enter an octal number: ");
                String octal = sc.nextLine();

                int decimal = Integer.parseInt(octal, 8);
                String hexadecimal = Integer.toHexString(decimal).toUpperCase();

                 System.out.println("Hexadecimal equivalent: " + hexadecimal);

                sc.close();
                }
        }

## 25. Hexadecimal to Octal
        import java.util.Scanner;

        public class HexToOctal {
            public static void main(String[] args) {
                Scanner sc = new Scanner(System.in);

                System.out.print("Enter a hexadecimal number: ");
                String hex = sc.nextLine();

                int decimal = Integer.parseInt(hex, 16);
                String octal = Integer.toOctalString(decimal);

                System.out.println("Octal equivalent: " + octal);

                sc.close();
            }
        }
