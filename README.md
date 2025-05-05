import java.time.LocalDate;
import java.time.format.DateTimeFormatter;

public class BirthdayGreeter {

    public static void wishBirthday(String name) {
        LocalDate today = LocalDate.now();
        DateTimeFormatter formatter = DateTimeFormatter.ofPattern("MMMM d");
        String formattedDate = today.format(formatter);

        System.out.println("Dear " + name + ",");
        System.out.println();
        System.out.println("Wishing you a very happy birthday!");
        System.out.println("May this " + formattedDate + " be filled with joy, laughter, and everything you've been wishing for.");
        System.out.println("Have a fantastic day!");
        System.out.println();
        System.out.println("Warmly,");
        System.out.println("Your Friend"); // You can customize this
    }

    public static void main(String[] args) {
        String birthdayPerson = "Alice"; // Replace with the actual name
        wishBirthday(birthdayPerson);
    }
}
