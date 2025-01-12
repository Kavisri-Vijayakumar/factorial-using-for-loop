import java.util.Scanner;
public class FactorialExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number to find its factorial: ");
        int number = scanner.nextInt();
        long factorial = 1;  
        if (number < 0) {
            System.out.println("Factorial is not defined for negative numbers.");
        } else {
            for (int i = 1; i <= number; i++) {
                factorial *= i; // Multiply factorial by current value of i
            }
            System.out.println("Factorial of " + number + " is: " + factorial);
        }
        scanner.close();
    }
}
output
Enter a number to find its factorial: 5
Factorial of 5 is: 120
