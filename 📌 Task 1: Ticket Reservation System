import java.util.*;

public class ReservationSystem {
    static Scanner sc = new Scanner(System.in);
    static String username = "admin", password = "1234";
    static String reservedPNR = "";

    public static void main(String[] args) {
        System.out.print("Enter Username: ");
        String user = sc.nextLine();
        System.out.print("Enter Password: ");
        String pass = sc.nextLine();

        if (user.equals(username) && pass.equals(password)) {
            System.out.println("\nLogin successful!");
            while (true) {
                System.out.println("\n1. Reserve Ticket");
                System.out.println("2. Cancel Ticket");
                System.out.println("3. Exit");
                System.out.print("Choose option: ");
                int choice = sc.nextInt();
                sc.nextLine();

                if (choice == 1) reserveTicket();
                else if (choice == 2) cancelTicket();
                else if (choice == 3) break;
                else System.out.println("Invalid option.");
            }
        } else System.out.println("Login failed.");
    }

    static void reserveTicket() {
        System.out.print("Enter Name: ");
        String name = sc.nextLine();
        System.out.print("Enter From: ");
        String from = sc.nextLine();
        System.out.print("Enter To: ");
        String to = sc.nextLine();
        System.out.print("Enter Date of Travel: ");
        String date = sc.nextLine();
        reservedPNR = "PNR" + (int)(Math.random() * 10000);
        System.out.println("Reservation successful. PNR: " + reservedPNR);
    }

    static void cancelTicket() {
        System.out.print("Enter your PNR to cancel: ");
        String pnr = sc.nextLine();
        if (pnr.equals(reservedPNR)) System.out.println("Ticket cancelled successfully!");
        else System.out.println("Invalid PNR.");
    }
}
