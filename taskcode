/**
 * Lucas M. T. Mauricio
 * Monday, June 14, 2021
 * Vending Machine ISU
 * This application imitates a vending machine. It prompts the user for a product they would like to purchase, the quantity of that product, and then how much money they will be using to pay.
 */

import java.util.Scanner;
import java.text.NumberFormat;

public class Main {

    public static void main(String[] args) {

        //The following code until line 43 makes up the structure of the vending machine
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############  ██╗  ██╗ ██████╗ ███╗   ██╗██████╗ ██╗███╗   ██╗██╗        ███████╗███╗   ██╗ █████╗  ██████╗██╗  ██╗███████╗  ###############");
        System.out.println("###############  ██║ ██╔╝██╔═══██╗████╗  ██║██╔══██╗██║████╗  ██║██║        ██╔════╝████╗  ██║██╔══██╗██╔════╝██║ ██╔╝██╔════╝  ###############");
        System.out.println("###############  █████╔╝ ██║   ██║██╔██╗ ██║██████╔╝██║██╔██╗ ██║██║        ███████╗██╔██╗ ██║███████║██║     █████╔╝ ███████╗  ###############");
        System.out.println("###############  ██╔═██╗ ██║   ██║██║╚██╗██║██╔══██╗██║██║╚██╗██║██║        ╚════██║██║╚██╗██║██╔══██║██║     ██╔═██╗ ╚════██║  ###############");
        System.out.println("###############  ██║  ██╗╚██████╔╝██║ ╚████║██████╔╝██║██║ ╚████║██║        ███████║██║ ╚████║██║  ██║╚██████╗██║  ██╗███████║  ###############");
        System.out.println("###############  ╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═══╝╚═════╝ ╚═╝╚═╝  ╚═══╝╚═╝        ╚══════╝╚═╝  ╚═══╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝  ###############");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");
        System.out.format("%17s %-70s %17s","###############  ", "\t\t\t\t\t\t\t\t\t\t\t\t\t Menu", "  ###############\n");
        System.out.format("%17s %-40s %-30s %35s %17s","###############  ", "Kani Roll", "  Salmon & Cheese Roll", "Kani Salad Roll", "  ###############\n");
        System.out.format("%17s %-45s %-25s %35s %17s","###############  ", "A1 ($5.50)", "  A2 ($6.50)", "A3 ($6.50)", "  ###############\n");
        System.out.format("%17s %-35s %-35s %-35s %17s","###############  ", "", "", "", "  ###############\n");
        System.out.format("%17s %-46s %-22s %37s %17s","###############  ", "Salmon Tempura Roll", "Pork Onigiri", "Salmon Onigiri", "  ###############\n");
        System.out.format("%17s %-47s %-23s %35s %17s","###############  ", "B1 ($7.50)", "B2 ($3.00)", "B3 (3.00)", "  ###############\n");
        System.out.format("%17s %-35s %-35s %35s %17s","###############  ", "", "", "", "  ###############\n");
        System.out.format("%17s %-42s %-28s %35s %17s","###############  ", "Miso Paste Onigiri", "Salmon w/ Mayo Onigiri", "Tuna w/ Mayo Onigiri", "  ###############\n");
        System.out.format("%17s %-47s %-23s %35s %17s","###############  ", "C1 ($3.00)", "C2 ($3.00) ", "C3 ($3.00)", "  ###############\n");
        System.out.format("%17s %-35s %-35s %35s %17s","###############  ", "", "", "", "  ###############\n");
        System.out.format("%17s %-45s %-25s %35s %17s","###############  ", "Matcha Mochi", "Strawberry Mochi", "Sakura Onigiri", "  ###############\n");
        System.out.format("%17s %-47s %-23s %35s %17s","###############  ", "D1 ($1.50)", "D2 ($1.50)", "D3 ($2.50)", "  ###############\n");
        System.out.format("%17s %-35s %-35s %35s %17s","###############  ", "", "", "", "  ###############\n");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");
        System.out.println("###############################################################################################################################################");

        //The following code until line 52 declares variables, a scanner and a currency format. It also declares constants for the prices of the products
        Scanner input = new Scanner(System.in);
        NumberFormat dollar = NumberFormat.getCurrencyInstance();
        String itemSelection;
        int productAmount;
        double finalTotal, inputMoney, remaining;
        final double KANI_ROLL = 5.5, SALMON_CC_ROLL = 6.5, KANI_SALAD_ROLL = 6.5, SALMON_TEMPURA_ROLL = 7.5, MATCHA_MOCHI = 1.5, STRAWBERRY_MOCHI = 1.5, SAKURA_MOCHI = 2.5;
        final int PORK_ONIGIRI = 3, SALMON_ONIGIRI = 3, MISO_PASTE_ONIGIRI = 3, SALMON_MAYO_ONIGIRI = 3, TUNA_MAYO_ONIGIRI = 3;

        //The following code until line 57 prompts the user for an item selection based on the number assigned to the item on the vending machine
        System.out.print("\nSelect your product: ");
        itemSelection = input.nextLine();
        itemSelection = itemSelection.toUpperCase();

        //The following if statements define what should be done depending on the item selected in line 56
        if(itemSelection.equals("A1")) {
            System.out.print("\nHow many Kani Rolls would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 71 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * KANI_ROLL;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".\n");

                //The following code until line 75 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 93 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                }
                else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                }
                else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                }
                else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if(itemSelection.equals("A2")){
            System.out.print("\nHow many Salmon Cream Cheese Rolls would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 107 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * SALMON_CC_ROLL;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 111 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 93 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("A3")){
            System.out.print("\nHow many Kani Salad Rolls would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 140 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * KANI_SALAD_ROLL;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 144 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 159 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("B1")){
            System.out.print("\nHow many Salmon Tempura Rolls would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 173 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * SALMON_TEMPURA_ROLL;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 177 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 192 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("Thanks for your purchase.\n");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("Thanks for your purchase.\n");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("B2")){
            System.out.print("\nHow many Pork Onigiris would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 206 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * PORK_ONIGIRI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 210 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 225 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("Thanks for your purchase.\n");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("Thanks for your purchase.\n");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("B3")){
            System.out.print("\nHow many Salmon Onigiris would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 239 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * SALMON_ONIGIRI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 243 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 228 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("C1")){
            System.out.print("\nHow many Miso paste Onigiris would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 272 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * MISO_PASTE_ONIGIRI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 276 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 292 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("C2")){
            System.out.print("\nHow many Salmon with Mayo Onigiris would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 305 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * SALMON_MAYO_ONIGIRI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 309 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 325 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("C3")){
            System.out.print("\nHow many Tuna with Mayo Onigiris would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 338 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * TUNA_MAYO_ONIGIRI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 342 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 358 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("D1")){
            System.out.print("\nHow many Matcha Mochis would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 371 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * MATCHA_MOCHI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 375 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 391 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("D2")){
            System.out.print("\nHow many Strawberry Mochis would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 404 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * STRAWBERRY_MOCHI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 408 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 424 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else if (itemSelection.equals("D3")){
            System.out.print("\nHow many Sakura Mochis would you like? ");
            productAmount = input.nextInt();

            //This if statement stops the user from inputting a number of products equal to or less than zero
            if (productAmount <= 0){
                System.out.print("Invalid input. Please enter a number of products equal to or greater than zero.");
            }
            else {
                //The following code until line 437 calculates and displays the total amount of money the user has to pay
                finalTotal = productAmount * SAKURA_MOCHI;
                System.out.println("Your total is " + dollar.format(finalTotal) + ".");

                //The following code until line 441 prompts the user for an amount of money which they will be using to pay for their product(s)
                System.out.print("Please enter the amount of money you will be using to pay: $");
                inputMoney = input.nextDouble();

                //The following code until line 457 controls what happens depending on how much money the user inputs
                if (inputMoney == finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    System.out.print("There is no change.");
                } else if (inputMoney > finalTotal) {
                    System.out.println("\nThanks for your purchase.");
                    remaining = inputMoney - finalTotal;
                    System.out.print("Your change is " + dollar.format(remaining) + ".");
                } else if (inputMoney < 0) {
                    System.out.print("\nInvalid input. The amount paid cannot be negative.");
                } else if (inputMoney < finalTotal) {
                    remaining = finalTotal - inputMoney;
                    System.out.println("You are " + dollar.format(remaining) + " short.");
                }
            }
        }
        else{
            //This line of code inform the user if they made an invalid input when selecting their product
            System.out.println("Invalid selection. Please select one of the options presented in the menu above.");
        }
    }
}
