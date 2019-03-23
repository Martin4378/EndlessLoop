# EndlessLoop

import java.util.Scanner;

public class P45_EndlessLoop {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String command;
        int min = Integer.MAX_VALUE;
        int max = Integer.MIN_VALUE;

        while (true) {
            command = scanner.nextLine();

            if (command.equalsIgnoreCase("end")) {
                break;
            }

            int currentNum = Integer.parseInt(command);

            if (currentNum < min) {
                min = currentNum;

            }
            if (currentNum > max){
                max = currentNum;

            }
        }

        System.out.printf("Max number: %d%n", max);
        System.out.printf("Min number: %d%n", min);
    }

}
