import java.util.Scanner;

public class GroceryListTracker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // Scanner for user input

        // Ask for number of items
        System.out.print("How many items do you want to add? ");
        int numItems = scanner.nextInt();
        scanner.nextLine(); // Consume leftover newline

        // Arrays to store item names and quantities
        String[] items = new String[numItems];
        int[] quantities = new int[numItems];

        // Loop to get user input for items
        for (int i = 0; i < numItems; i++) {
            System.out.print("Enter name of item " + (i + 1) + ": ");
            items[i] = scanner.nextLine(); // Get item name

            System.out.print("Enter quantity of " + items[i] + ": ");
            quantities[i] = scanner.nextInt(); // Get quantity
            scanner.nextLine(); // Consume leftover newline
        }

        // Display the grocery list
        System.out.println("\nGrocery List:");
        for (int i = 0; i < numItems; i++) {
            System.out.println((i + 1) + ". " + items[i] + " - " + quantities[i]);
        }
    }
}
# Touchstone-final-project
Touchstone 4 final project
