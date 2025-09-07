# Conventional vs Urdhva Thiryagbhyam Vedic Multiplication Benchmark Using Python

This repository contains a comprehensive benchmark comparing **conventional multiplication** using Python’s built-in operator to the traditional **Urdhva Thiryagbhyam Vedic multiplication** method. The Vedic method implements the ancient "Vertical and Crosswise" technique, manually handling digit-wise multiplication and carries.

---

## Demonstration of Multiplication Methods

The following examples show that both the conventional and Vedic methods yield identical results, verifying the correctness of the Vedic implementation:

| Example       | Conventional Result | Vedic Result | Agreement       |
|---------------|---------------------|--------------|-----------------|
| 3 × 7         | 21                  | 21           | Both methods agree!  |
| 9 × 8         | 72                  | 72           | Both methods agree!  |
| 23 × 45       | 1035                | 1035         | Both methods agree!  |
| 123 × 456     | 56088               | 56088        | Both methods agree!  |
| 99 × 99       | 9801                | 9801         | Both methods agree!  |
| 12 × 34       | 408                 | 408          | Both methods agree!  |

---

## Correctness Verification

- 30 different test cases were verified.
- **All tests passed**, confirming the Vedic method produces correct multiplication results as compared to the conventional method.

---

## Performance Benchmarking

Performance was tested across various number ranges, timing average execution per multiplication over 10,000 iterations:

| Number Range       | Conventional Time (s) | Vedic Time (s) | Performance Ratio (Vedic / Conventional) | Speed Comparison          |
|--------------------|----------------------|----------------|------------------------------------------|---------------------------|
| 1 to 9             | 0.00000012           | 0.00000341     | 28.10x                                   | Vedic is 28.10x slower    |
| 10 to 99           | 0.00000011           | 0.00000572     | 50.27x                                   | Vedic is 50.27x slower    |
| 100 to 999         | 0.00000014           | 0.00000869     | 61.07x                                   | Vedic is 61.07x slower    |
| 1000 to 9999       | 0.00000012           | 0.00001214     | 105.02x                                  | Vedic is 105.02x slower   |
| 10000 to 99999     | 0.00000013           | 0.00001743     | 132.67x                                  | Vedic is 132.67x slower   |

---

## Overall Performance Summary

- **Conventional average time:** 0.00000012 seconds per operation.
- **Vedic average time:** 0.00000948 seconds per operation.
- **Overall performance ratio:** Vedic method is approximately **75.89x slower** than conventional multiplication.

---

## Analysis Summary & Observations

1. **Conventional Multiplication:**
   - Utilizes Python’s built-in `*` operator.
   - Highly optimized at the C language level.
   - Consistently very fast across all tested number sizes.
   - Handles all edge cases automatically and efficiently.

2. **Urdhva Thiryagbhyam Vedic Method:**
   - Implements the traditional "Vertical and Crosswise" digit-by-digit multiplication technique.
   - Requires manual carry management and string manipulation.
   - Involves more computational steps due to per-digit processing.
   - Less efficient in terms of speed compared to the built-in multiplication operator.

---

## Usage

- The main script (`Benchmarking.ipynb`) demonstrates the multiplication methods, verifies correctness, and runs detailed performance benchmarks.
- Ideal for educational purposes and exploring classical multiplication techniques versus modern optimized operations.

---

## License

MIT

---
