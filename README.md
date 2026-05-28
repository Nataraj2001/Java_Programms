# Java_Programms
## Reverse a String
String str = "Happy Coidng";
        String rev = " ";
        for (int i = str.length()-1; i >=0; i--){
            rev = rev + str.charAt(i);
        }
        System.out.println("Reverse String is:" + rev);

## Palindrome 
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

## Swap two numbers
 int a  = 10;
        int b = 20;
        int temp;
        temp = a;
        a = b;
        b = temp;
            System.out.println(a + " " + b);
        }
## Even and Odd Number
  int num = 10;
       if(num % 2 == 0){
           System.out.println("Even number");
       }else{
            System.out.println("Odd number");
       }

## Prime Number Check
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


