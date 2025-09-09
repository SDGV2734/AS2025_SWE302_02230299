# Software Testing Practical 3: Specification-Based Testing with Equivalence Partitions and Boundary Values

## Key Concepts Covered

### Specification-Based Testing

Tests are designed based on the requirements/specifications, not the implementation. This ensures that the software behaves as expected from a user's perspective.

### Equivalence Partitioning

The input space is divided into partitions (groups) where the system should behave similarly. By testing one value from each partition, you minimize the number of test cases while maximizing coverage.

### Boundary Value Analysis (BVA)

Special attention is given to values at the edges of partitions, as these are common sources of bugs (e.g., off-by-one errors).

### Decision Table Testing

All possible combinations of inputs and their expected outcomes are systematically tested, ensuring thorough coverage of business rules.

### Systematic, Critical Thinking

Testing is planned and methodical, preventing random/ad hoc approaches. This leads to robust, comprehensive test suites.

---

## Shipping Fee V2: Partitions & Boundaries

### Equivalence Partitions

#### Weight

- **Invalid (≤ 0):** Examples: -5, 0
- **Valid Standard (0 < w ≤ 10):** Examples: 1, 10
- **Valid Heavy (10 < w ≤ 50):** Examples: 20, 50
- **Invalid (> 50):** Examples: 51, 100

#### Zone

- **Valid Zones:** "Domestic", "International", "Express"
- **Invalid Zones:** "Local", "", "domestic" (case sensitive)

#### Insured

- **Not Insured:** false
- **Insured:** true

### Boundary Values

#### Weight

- **Lower boundary:** 0 (invalid), 0.01 (just valid)
- **Mid boundary:** 10 (last Standard), 10.01 (first Heavy)
- **Upper boundary:** 50 (valid), 50.01 (invalid)

#### Zone

- Not numerical; test all valid zones and at least one invalid zone.

#### Insured

- Boolean; test both `true` and `false` values.

---

## Why Use These Test Cases?

- **Equivalence Partitions:** Ensure all types of input are covered, verifying general system behavior.
- **Boundary Values:** Detect edge-case and off-by-one errors, which are common in real-world bugs.
- **Combined Approach:** Results in a robust, requirement-driven test suite that maximizes coverage and reliability.

---

## Submission Checklist

- [x] Screenshot of all tests passing

![alt text](image1.png)

-  All code files: `shipping_v2.go`, `shipping_v2_test.go` 

[HERE!!](https://github.com/SDGV2734/SWE302_shipping_test_practical_3.git)
