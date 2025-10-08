# Additional Practice Problems - Chapter 2: Representing and Manipulating Information

## 1. Bit-Level Operations and Boolean Algebra
Evaluate the following expressions where x = 0x5A and y = 0x3C:
- a) x & y
- b) x | y  
- c) x ^ y
- d) ~x & 0xFF
- e) (x << 2) & 0xFF

## 2. Two's Complement Arithmetic
For w = 6 bits, determine if the following additions result in overflow:
- a) 15 + 12
- b) -20 + -15
- c) 25 + 7
- d) -16 + 10

## 3. Unsigned vs Signed Comparisons
Given x = 0x80000000 and y = 0x7FFFFFFF (32-bit values), evaluate:
- a) x < y (signed comparison)
- b) x < y (unsigned comparison)
- c) (int)x < (int)y
- d) (unsigned)x < (unsigned)y

## 4. Bit Shifting Operations
For x = 0xC3A5 (16-bit value):
- a) x >> 3 (arithmetic right shift)
- b) x >> 3 (logical right shift)
- c) x << 4
- d) What happens to the sign bit in each case?

## 5. Floating Point Representation
Convert the following to IEEE 754 single-precision format (show in hex):
- a) 0.375
- b) -12.5
- c) 1024.0

## 6. Floating Point Special Cases
Identify what each IEEE 754 single-precision value represents:
- a) 0x7F800000
- b) 0xFF800000
- c) 0x7FC00000
- d) 0x00000000
- e) 0x80000000

## 7. Integer Encoding Practice
Fill in the table for w = 12 bits:

| Binary          | Decimal (unsigned) | Decimal (signed) | Hexadecimal |
|-----------------|-------------------|------------------|-------------|
| 101011001100    |                   |                  |             |
|                 | 2847              |                  |             |
|                 |                   | -1249            |             |
|                 |                   |                  | 0x7A3       |

## 8. Byte Ordering (Endianness)
A 32-bit integer 0x12345678 is stored at address 0x100. Show the byte layout for:

| Address | Big-endian | Little-endian |
|---------|------------|---------------|
| 0x100   |            |               |
| 0x101   |            |               |
| 0x102   |            |               |
| 0x103   |            |               |

## 9. Floating Point Precision
Explain why the following C code might not work as expected:
```c
float x = 1e20;
float y = 1e20 + 1.0;
if (x == y) printf("Equal\n");
else printf("Not equal\n");
```

## 10. Bit Manipulation Puzzles
Write expressions using only bit-level operations (&, |, ^, ~, <<, >>) and constants:
- a) Set bit position k in integer x
- b) Clear bit position k in integer x  
- c) Test if bit position k is set in integer x
- d) Count the number of 1 bits in integer x (population count)

## 11. Overflow Detection
Write a function that detects if adding two signed integers will cause overflow:
```c
int add_overflow(int x, int y) {
    // Your code here - use only bit operations
}
```

## 12. Floating Point Comparison
Given these IEEE 754 single-precision values, order them from smallest to largest:
- a) 0x3F800000
- b) 0xBF800000  
- c) 0x40000000
- d) 0x00000000
- e) 0x7F7FFFFF

## 13. Machine-Level Data Sizes
On a 64-bit x86-64 machine, what are the sizes (in bytes) of:
- a) char
- b) short
- c) int
- d) long
- e) long long
- f) float
- g) double
- h) pointer

## 14. Casting and Truncation
What are the results of these operations on a 32-bit machine?
```c
int x = -1;
unsigned u = 2147483648U; // 2^31
```
- a) (unsigned) x
- b) (int) u
- c) (short) x
- d) (unsigned short) u

## 15. IEEE 754 Denormalized Numbers
Explain what denormalized numbers are and give an example of the smallest positive denormalized number in IEEE 754 single-precision format.

## 16. Bitwise Logical vs Arithmetic Operations
For x = 0xAB and y = 0x3F, calculate:
- a) x && y
- b) x || y
- c) !x
- d) x & y
- e) x | y
- f) ~x

## 17. Sign Extension
Show the result of sign-extending the following 8-bit values to 16 bits:
- a) 0x7F
- b) 0x80
- c) 0xFF
- d) 0x01

## 18. Floating Point Rounding
Convert the following decimal numbers to IEEE 754 single-precision, showing any rounding that occurs:
- a) 1/3
- b) 0.1
- c) 16777217 (2^24 + 1)

## 19. Modular Arithmetic
For 4-bit two's complement representation:
- a) What is the range of representable values?
- b) Calculate: 7 + 6
- c) Calculate: -5 + -7
- d) Calculate: 4 × 3

## 20. Hexadecimal Practice
Convert between representations:

| Decimal | Binary    | Hexadecimal | Octal |
|---------|-----------|-------------|-------|
| 255     |           |             |       |
|         | 10101010  |             |       |
|         |           | 0xDEAD      |       |
|         |           |             | 377   |
