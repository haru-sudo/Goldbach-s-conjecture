# Goldbach Conjecture Solver

This Python script calculates and verifies Goldbach's Conjecture for all even numbers up to a user-defined target sum. The results are saved in a text file called `Goldbach-conjecture.txt`.

## Overview

Goldbach's Conjecture is an unproven theory in mathematics which states that every even integer greater than 2 can be expressed as the sum of two prime numbers. This script implements the Sieve of Eratosthenes algorithm to generate a list of prime numbers and then tests the conjecture for all even numbers up to a specified target sum.

## Features

- **Prime Number Generation**: Uses the Sieve of Eratosthenes to efficiently generate all prime numbers up to the target sum.
- **Goldbach Conjecture Verification**: For every even number from 4 to the target sum, the script checks if it can be expressed as the sum of two primes.
- **File Output**: The results are written to a file called `Goldbach-conjecture.txt`, with each line showing an even number as the sum of two prime numbers.

## How It Works

1. **Sieve of Eratosthenes**: The `sieve_of_eratosthenes` function generates all prime numbers up to the given target sum.
2. **Goldbach Conjecture**: The `goldbach_conjecture` function iterates through all even numbers from 4 to the target sum. For each even number, it checks if it can be written as the sum of two primes from the list generated by the sieve.
3. **Output**: The results are saved to `Goldbach-conjecture.txt` in the format `even_number = prime1 + prime2`.

## Usage

1. Clone the repository or download the script.
2. Run the script using Python:

    ```bash
    python goldbach_conjecture.py
    ```

3. Enter the target sum when prompted:

    ```bash
    Total to be sought>>
    ```

4. The results will be written to `Goldbach-conjecture.txt`.

## Example

If you input `20` as the target sum, the script will verify the conjecture for all even numbers from 4 to 20, producing an output similar to the following in `Goldbach-conjecture.txt`:

```
4 = 2 + 2
6 = 3 + 3
8 = 3 + 5
10 = 3 + 7
12 = 5 + 7
14 = 3 + 11
16 = 3 + 13
18 = 5 + 13
20 = 3 + 17
```

## Requirements

- Python 3.x

No additional libraries are required.

## License

This project is licensed under the MIT License.

## Acknowledgments

- The Sieve of Eratosthenes algorithm for generating prime numbers.
- Goldbach's Conjecture, an unsolved problem in number theory that continues to intrigue mathematicians.
