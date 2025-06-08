# Bitwise-matching-pattern
# Next Number with Same Number of 1s

## Description
This Python program finds the next larger integer that has exactly the same number of 1 bits in its binary representation as the input number.

## Features
- Finds the next larger number with matching 1-bit count
- Handles positive integers
- Includes clear test cases with binary representations
- Simple and easy to understand implementation

## Requirements
- Python 3.x
- No external dependencies needed

## How to Use

1. Save the code to a file (e.g., `next_number.py`)
2. Run the script:
```bash
python next_number.py
```

3. To use in your own code:
```python
from next_number import next_number_with_same_ones

result = next_number_with_same_ones(6)  # Returns 9
```

## Functions

### `count_ones(number)`
- Counts how many 1's are in the binary version of a number
- Uses bitwise operations for efficient counting

### `next_number_with_same_ones(input_num)`
- Finds the next bigger number with the same number of 1's
- Returns -1 if no such number exists or for invalid input
- Includes safety check to prevent infinite loops

## Test Cases
The program includes 2 clear test cases:

1. Input: 6 (binary: 0b110)
   - Output: 9 (binary: 0b1001)

2. Input: 13 (binary: 0b1101) 
   - Output: 14 (binary: 0b1110)

## Example Usage
```python
# Find next number after 5
print(next_number_with_same_ones(5))  # Output: 6 (101 → 110)

# Find next number after 9
print(next_number_with_same_ones(9))  # Output: 10 (1001 → 1010)
```

## Algorithm
1. Count the 1 bits in the input number
2. Check each subsequent number until finding one with the same count
3. Return the first matching number found

## Limitations
- Only works for positive integers
- Returns -1 for negative inputs
- Has an upper limit of 1,000,000 to prevent infinite loops

## License
MIT License - Free to use and modify
