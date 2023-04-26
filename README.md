# Assignment
A program that prompts the user to input a series of positive integers until a negative integer is entered. The program should calculate and display the sum of all the positive integers that were entered.

import java.util.Scanner;

public class PositiveIntegerSum {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        int sum = 0;
        int num;

        System.out.println("Enter positive integers (enter a negative integer to stop):");

        do {
            num = input.nextInt();

            if (num >= 0) {
                sum += num;
            }
        } while (num >= 0);

        System.out.println("The sum of the positive integers entered is: " + sum);
    }
}
