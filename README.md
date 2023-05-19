# Coin Change Calculation

This C program calculates the minimum number of coins required to make up a given amount of change. It asks the user for the amount in cents that needs to be given as change and then calculates the number of quarters, dimes, nickels, and pennies required.

## Usage

1. Compile the program using a C compiler of your choice (e.g., GCC).
2. Run the compiled executable.
3. Enter the amount of change owed in cents when prompted.
4. The program will display the total number of coins required to make up the change.

## Program Logic

The program follows a simple logic to calculate the number of coins for each denomination:

1. The program prompts the user to enter the amount of change owed.
2. The `get_cents()` function takes user input and validates it to ensure a positive value is entered.
3. The program then calculates the number of quarters by dividing the remaining amount of change by 25 (since 1 quarter equals 25 cents).
4. The same process is repeated for dimes, nickels, and pennies, using their respective denominations (10, 5, and 1).
5. The total number of coins is calculated by summing the quantities of each type of coin.
6. Finally, the program prints the total number of coins required to make up the change.

## Functions

1. `get_cents()`: This function takes user input for the amount of change owed and returns the validated value. It ensures that a non-negative integer is entered.
2. `calculate_quarters(cents)`: This function calculates the number of quarters required based on the remaining amount of change.
3. `calculate_dimes(cents)`: This function calculates the number of dimes required based on the remaining amount of change.
4. `calculate_nickels(cents)`: This function calculates the number of nickels required based on the remaining amount of change.
5. `calculate_pennies(cents)`: This function returns the remaining amount of change as pennies.

## Example

Suppose the user enters "73" as the amount of change owed. The program will calculate the minimum number of coins required as follows:

- Quarters: 2 (50 cents)
- Dimes: 2 (20 cents)
- Nickels: 0 (0 cents)
- Pennies: 3 (3 cents)

The program will then display the total number of coins required as 7.
