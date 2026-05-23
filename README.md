# prime-numbers-up-to-n
A simple Java program that prints all prime numbers up to a given number using nested loops.

import java.util.Scanner;
public class PrimeNumbersUpToN {
    static void printPrimeNumbers(int n) {
        for (int i = 2; i <= n; i++) {
            int count = 0;
            for (int j = 1; j <= i; j++) {
                if (i % j == 0) {
                    count++;
                }
            }
            if (count == 2) {
                System.out.print(i + " ");
            }
        }
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
        printPrimeNumbers(n);
    }
}
