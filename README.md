# Calculator
A simple calculator, takes 2 number from the user (a &amp; b) and an operation as follows:
+ for addition
- for subtraction
* for multiplication
/ for division
% for reminder

import java.util.*;
public class Calculator{

    public static void main(String args[]){
        Scanner sc= new Scanner(System.in);
        int a;
        int b;
        char ch;
        int choice;

        do{
         a=sc.nextInt();
         ch=sc.next().charAt(0);
         b=sc.nextInt();
         

        switch(ch){
            case '+': System.out.println(a+b);
            break;
            case '-': System.out.println(a-b);
            break;
            case '*': System.out.println(a*b);
            break;
            case '/':if(b==0){
                         System.out.println("invalid");  
                    }else{
                         System.out.println(a/b);
                    }
            break;
            case '%':if(b==0){
                         System.out.println("invalid");
                    }else{
                         System.out.println(a%b);}
            break;
            default: System.out.println("invald entry");
          }
          System.out.println("do you want to continue? (yes(1) no(0))");
          choice=sc.nextInt();
          
         }while(choice==1);
       
    }
}
