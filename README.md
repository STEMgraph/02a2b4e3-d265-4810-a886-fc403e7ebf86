<!---
{
  "id": "02a2b4e3-d265-4810-a886-fc403e7ebf86",
  "depends_on": [],
  "author": "Stephan Bökelmann",
  "first_used": "2025-05-02",
  "keywords": ["numbers", "binary", "decimal", "hexadecimal"]
}
--->

# Number Systems: Binary, Decimal, and Hexadecimal

> In this exercise you will learn how to represent natural numbers in binary, decimal, and hexadecimal systems. Furthermore we will explore how to convert numbers between these systems, and how basic operations like addition and multiplication are performed in each base.

### Introduction

The way humans write numbers has evolved through centuries. The decimal system (base-10) is the most familiar, using ten digits (0 to 9), and traces its roots to ancient civilizations like the Egyptians and the Hindus, likely influenced by counting with ten fingers. In contrast, computers use the binary system (base-2), employing only two digits, 0 and 1. This binary representation aligns perfectly with the digital electronic world, where two voltage levels (e.g., on/off) encode information.

Another useful system in computing is hexadecimal (base-16), which employs sixteen symbols: 0–9 and A–F. It serves as a compact and human-friendly representation of binary-coded data, grouping binary digits into clusters of four (e.g., 1111₂ = F₁₆).

All number systems rely on the same underlying concept: **positional value**. A number is expressed as the sum of its digits multiplied by the base raised to powers corresponding to their positions. For instance:

```
Decimal:     345 = 3×10^2 + 4×10^1 + 5×10^0
Binary:     1011 = 1×2^3 + 0×2^2 + 1×2^1 + 1×2^0 = 11 in decimal
Hex:         1F = 1×16^1 + 15×16^0 = 31 in decimal
```

Understanding these systems and switching between them is crucial in computer science, digital electronics, and cybersecurity.

### Further Readings and Other Sources

* [Number Systems – Khan Academy](https://www.khanacademy.org/computing/computer-science/cryptography)
* [Binary and Hexadecimal Number Systems](https://doi.org/10.1109/9780470544334.ch1)
* [Computerphile: Hexadecimal](https://www.youtube.com/watch?v=obXH0GxNAMk)
* [Understanding Binary - Stanford CS](https://cs.stanford.edu/people/eroberts/courses/soco/projects/2000-01/digital-watch/binary.html)

### Tasks

#### Task 1: Converting Between Number Systems

In this task, you will practice converting natural numbers between binary, decimal, and hexadecimal forms. Each conversion requires understanding the place value system used in each base.

1. **Convert 45 in decimal to binary and hexadecimal**:

   * **To Binary**: Repeatedly divide the number by 2, noting the remainders. Reverse the sequence of remainders to get the binary number.

     * 45 ÷ 2 = 22 remainder 1
     * 22 ÷ 2 = 11 remainder 0
     * 11 ÷ 2 = 5 remainder 1
     * 5 ÷ 2 = 2 remainder 1
     * 2 ÷ 2 = 1 remainder 0
     * 1 ÷ 2 = 0 remainder 1 → Read upwards: 101101₂
   * **To Hexadecimal**: Divide the decimal number by 16.

     * 45 ÷ 16 = 2 remainder 13 → 13 corresponds to D → Hex = 2D₁₆

2. **Convert 11011 in binary to decimal and hexadecimal**:

   * **To Decimal**: Use positional values from right to left.

     * 1×2⁴ + 1×2³ + 0×2² + 1×2¹ + 1×2⁰ = 16 + 8 + 0 + 2 + 1 = 27₁₀
   * **To Hexadecimal**: Group binary digits into 4s from the right: 0001 1011 → 1B₁₆

3. **Convert 7F in hexadecimal to binary and decimal**:

   * **To Binary**: 7 = 0111, F = 1111 → Binary = 01111111₂
   * **To Decimal**: 7×16 + 15 = 112 + 15 = 127₁₀

#### Task 2: Addition Across Number Systems

In this task, we will perform additions in binary, hexadecimal, and decimal systems, showing intermediate steps and equivalent values.

1. **Add 1011₂ and 1101₂**:

   * Convert to decimal: 1011 = 11, 1101 = 13
   * Add: 11 + 13 = 24
   * Convert the sum back to binary: 24 ÷ 2 → 11000₂

2. **Add 3A₁₆ and 29₁₆**:

   * Convert to decimal: 3A = 58, 29 = 41
   * Add: 58 + 41 = 99
   * Convert to hexadecimal: 99 ÷ 16 = 6 remainder 3 → 63₁₆

3. **Add 58₁₀ and 74₁₀**:

   * Perform direct addition: 58 + 74 = 132
   * Convert to binary: 10000100₂
   * Convert to hexadecimal: 132 ÷ 16 = 8 remainder 4 → 84₁₆

#### Task 3: Multiplication Across Number Systems

In this task, we will multiply numbers in each system and convert the result into all three formats.

1. **Multiply 101₂ and 11₂**:

   * Convert to decimal: 101 = 5, 11 = 3
   * Multiply: 5 × 3 = 15
   * Convert result to binary: 1111₂

2. **Multiply A₁₆ and 4₁₆**:

   * Convert to decimal: A = 10, 4 = 4
   * Multiply: 10 × 4 = 40
   * Convert to hexadecimal: 28₁₆

3. **Multiply 13₁₀ and 6₁₀**:

   * Multiply: 13 × 6 = 78
   * Convert to binary: 1001110₂
   * Convert to hexadecimal: 78 ÷ 16 = 4 remainder 14 → 4E₁₆

### Questions

1. What is the base of the decimal, binary, and hexadecimal systems?
2. What are the digits available in hexadecimal?
3. How is the number 255 represented in binary and hexadecimal?
4. Convert the binary number 100101 to decimal.
5. Convert the hexadecimal number B3 to decimal.
6. How do you add two binary numbers? Show an example.

### Advice

Understanding number systems takes time and practice, especially if you're new to binary or hexadecimal representations. Work through conversions methodically and double-check your intermediate results, particularly powers of two or sixteen. Use your calculator only to verify results after doing them by hand. Visual aids such as grouping binary digits when converting to hexadecimal can make the process easier. If this sheet was challenging, consider reviewing the [Number Systems Basics](#) sheet before proceeding to advanced topics like floating-point representation or base arithmetic.
