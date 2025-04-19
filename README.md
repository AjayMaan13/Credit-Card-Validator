# Credit Card Validator

This project is a C program that validates credit card numbers using **Luhn’s Algorithm** and identifies the type of card based on number patterns. It runs in a continuous loop, asking for user input until the user chooses to exit by entering `0`.

## 🔍 Overview

Credit card numbers follow specific structures and include a built-in checksum. This program checks the validity of a credit card number using:

- **Luhn’s Algorithm** for checksum validation
- Specific starting digit patterns to identify the card issuer:
  - American Express: starts with 34 or 37, 15 digits long
  - MasterCard: starts with 51–55, 16 digits long
  - Visa: starts with 4, 13 or 16 digits long

## 💡 Features

- Repeatedly prompts the user for credit card numbers.
- Input validation ensures only valid numbers are processed:
  - **Handles invalid input**, including strings and negative numbers.
  - **Continues until `0` is entered to exit** the program.
- Validates credit card numbers based on:
  - **Luhn’s checksum**
  - **Length and starting digits**
- Identifies and prints the card type:
  - `AMEX` for American Express cards
  - `MASTERCARD` for MasterCard cards
  - `VISA` for Visa cards
  - Or prints `INVALID` if the number doesn't match any criteria

## 🧪 Example Usage

```bash
$ ./credit
Enter Card Number (0 to exit): 4003600000000014
VISA
Enter Card Number (0 to exit): asf
Enter Card Number (0 to exit): 400000000
INVALID
Enter Card Number (0 to exit): 0
Exiting program.
