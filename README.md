# Jawa.2
currency converter 


import java.util.Scanner;

public class CurrencyConverter {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Currency Converter");

        System.out.println("1. INR to USD");
        System.out.println("2. USD to INR");
        System.out.println("3. INR to EUR");

        System.out.print("Choose option: ");
        int choice = sc.nextInt();

        System.out.print("Enter amount: ");
        double amount = sc.nextDouble();

        double result = 0;

        switch (choice) {

            case 1:
                result = amount * 0.012;
                System.out.println("Converted Amount: " + result + " USD");
                break;

            case 2:
                result = amount * 83;
                System.out.println("Converted Amount: " + result + " INR");
                break;

            case 3:
                result = amount * 0.011;
                System.out.println("Converted Amount: " + result + " EUR");
                break;

            default:
                System.out.println("Invalid choice");
        }

        sc.close();
    }
