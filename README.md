import java.util.*;

public class Main{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Enter first number (a):");
        double a = sc.nextDouble();
        System.out.println("Enter second number (b):");
        double b = sc.nextDouble();
        
        System.out.println("Choose an operation:");
        System.out.println("1. +(Addition)");
        System.out.println("2. -(Subtractiion)");
        System.out.println("3. *(Multiplication)");
        System.out.println("4. /(Divison)");
        System.out.println("5. %(Modulo or Remainder)");
        
        System.out.println("Choose your choice:");
        int choice = sc.nextInt();
        
        double result;
        switch (choice) {
            case 1 :
                result = a + b;
                System.out.println(a+"+"+b+"="+result);
                break;
            case 2 :
                result = a - b;
                System.out.println(a+"-"+b+"="+result);
                break;
            case 3 :
                result = a * b;
                System.out.println(a+"*"+b+"="+result);
                break;
            case 4 :
                if (b==0) {
                    System.out.println("Error:not defined value due to zero in denominator");
                } else {
                    result = a / b;
                    System.out.println(a+"/"+b+"="+result);
                    break;
                }
            case 5 :
                result = a % b ;
                System.out.println(a+"%"+b+"="+result);
                break;
        }
        
    }
}
