# program2.java
# generates a series of numbers

import java.util.Scanner;

public class NumberSeries {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the value of 'x': ");
        int x = scanner.nextInt();

        // Generate the number series
        StringBuilder output = new StringBuilder();
        for (int i = 1; i <= x; i++) {
            output.append(i);
            if (i != x) {
                output.append(", ");
            }
        }

        System.out.println("Output: " + output);

        scanner.close();
    }
}
