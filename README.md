---

# Luhn Algorithm

## Overview

The Luhn algorithm, also known as the Luhn formula or modulus 10 algorithm, is a simple checksum formula used to validate a variety of identification numbers, such as credit card numbers, IMEI numbers, National Provider Identifier numbers, and Canadian Social Insurance Numbers.

## How It Works

1. **Step 1: Reverse the Number**: Reverse the digits of the identification number.

2. **Step 2: Double Every Second Digit**: Starting from the rightmost digit (which is the check digit), double the value of every second digit. If the doubled value is greater than or equal to 10, subtract 9 from the result.

3. **Step 3: Sum All Digits**: Sum all the digits of the modified identification number, including the check digit.

4. **Step 4: Validate**: If the total sum is divisible by 10 (i.e., the modulo 10 operation yields 0), then the identification number is valid according to the Luhn algorithm.

## Code Explanation

The provided Python code implements the Luhn algorithm to verify the validity of a credit card number.

- **`verify_card_number(card_number)`:** This function takes a credit card number as input, applies the Luhn algorithm to verify its validity, and returns a boolean value indicating whether the card number is valid or not.

- **`main()`:** This function serves as the entry point of the program. It initializes a sample credit card number, removes any hyphens or spaces from the number, and then calls the `verify_card_number` function to check its validity. Based on the result, it prints either "VALID!" or "INVALID!".

## Usage

To use the provided code:

1. Replace the `card_number` variable with the credit card number you want to verify.

2. Run the `main()` function.

3. The program will output either "VALID!" or "INVALID!" based on the validity of the credit card number.

## Note

- The Luhn algorithm provides a simple and effective method for quickly verifying the validity of identification numbers, particularly credit card numbers.
- While the Luhn algorithm can detect most common errors, it is not foolproof and may not catch all types of errors or fraud.

---
