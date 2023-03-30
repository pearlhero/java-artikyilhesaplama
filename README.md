# java-artikyilhesaplama
java-artikyilhesaplama

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Yıl giriniz : ");
        int year = input.nextInt();

        if ((year % 4 == 0 && year % 100 !=0 && year > 0) || (year % 400 == 0)) {
        System.out.println(year + " artık bir yıldır.");
        } else if (year > 0) {
            System.out.println(year + " artık bir yıl değildir.");
        }else {
            System.out.println("Hatalı bir yıl girdiniz. Lütfen tekrar deneyiniz !");
        }
    }
}
