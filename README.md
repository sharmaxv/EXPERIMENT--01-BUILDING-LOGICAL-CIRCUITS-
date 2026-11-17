# EXPERIMENT-01: BUILDING LOGICAL CIRCUITS

## 1. Aim

To design, implement, simplify, and verify combinational logic circuits using Boolean algebra and digital logic gates.

## 2. Boolean Notation

Use the following notation throughout this experiment:

| Symbol | Meaning | Example |
|---|---|---|
| `!A` | NOT A | `!A` |
| `A & B` | AND | `A & B` |
| `A \| B` | OR | `A \| B` |
| `A ^ B` | XOR | `A ^ B` |
| `A XNOR B` | XNOR | `A XNOR B` |

**Important:** In these equations, `!` means NOT, `&` means AND, `|` means OR, and `^` means XOR. Parentheses determine the order of operations.

## 3. Advanced Boolean Equations

### Equation 1: Four-Input Sum-of-Products

```text
F1 = (!A & B & C)
   | (A & B & !D)
   | (!B & C & D)
   | (A & !C & D)
```

**Inputs:** A, B, C, D  
**Output:** F1  
**Challenge:** Simplify the expression and compare gate counts.

### Equation 2: Product-of-Sums Circuit

```text
F2 = (A | !B | C)
   & (!A | B | D)
   & (B | !C | !D)
```

**Inputs:** A, B, C, D  
**Output:** F2  
**Challenge:** Implement the circuit using NAND gates and verify functional equivalence.

### Equation 3: Nested Complement Logic

```text
F3 = !(
       ((! (A | B)) | (C & D))
       &
       (A | (!(B | C)))
     )
```

**Inputs:** A, B, C, D  
**Output:** F3  
**Challenge:** Apply De Morgan's theorems and implement the circuit using NAND and NOR gates.

### Equation 4: XOR-XNOR Combinational Circuit

```text
F4 = ((A XOR B) & (C XNOR D))
   | (!A & B & (C XOR D))
```

**Inputs:** A, B, C, D  
**Output:** F4  
**Challenge:** Compare an XOR/XNOR implementation with a basic-gate implementation.

### Equation 5: Five-Input Logic Function

```text
F5 = (A & B & !C)
   | (!A & D & E)
   | (B & C & !E)
   | (!B & C & D)
```

**Inputs:** A, B, C, D, E  
**Output:** F5  
**Challenge:** Generate and verify all 32 input combinations.

### Equation 6: Six-Input Mixed Logic

```text
F6 = ((A | B) & !(C | D))
   | ((C XOR E) & (D | G))
   | (!A & B & E)
```

**Inputs:** A, B, C, D, E, G  
**Output:** F6  
**Challenge:** Calculate gate count and logic depth. Verify all 64 input combinations.

### Equation 7: NAND-NOR Hybrid Logic

```text
F7 = (! (A & B) & !(C | D))
   | (!(A | C) & B & D)
```

**Inputs:** A, B, C, D  
**Output:** F7  
**Challenge:** Implement the function using NAND and NOR gates with any required input inversions.

### Equation 8: Six-Input Advanced Combinational Logic

```text
F8 = ((A XOR B) & (C XNOR D))
   | (!(A | B) & C & E)
   | (A & B & !(D | F))
```

**Inputs:** A, B, C, D, E, F  
**Output:** F8  
**Challenge:** Simplify the expression, design the circuit, and verify all 64 input combinations.

## 4. Experimental Procedure

1. Identify all input variables and the output.
2. Draw the logic circuit for each equation.
3. Implement the circuit in Logisim Evolution, Proteus, or a digital logic trainer kit.
4. Apply all possible input combinations.
5. Record the expected and observed outputs.
6. Simplify the Boolean expression using Boolean algebra.
7. Build the simplified circuit and compare gate counts.
8. Save the circuit diagrams, truth tables, and verification screenshots.

## 5. Truth Table Requirements

| Number of inputs | Required combinations |
|---:|---:|
| 4 | 16 |
| 5 | 32 |
| 6 | 64 |

Use this format to record the results:

| Inputs | Expected output | Observed output | Status |
|---|---|---|---|
| 0000 |  |  |  |
| 0001 |  |  |  |
| 0010 |  |  |  |
| ... |  |  |  |

Extend the table to include every input combination required by each equation.

## 6. Performance Analysis

For each circuit, record:

- Number of AND gates
- Number of OR gates
- Number of NOT gates
- Number of XOR/XNOR gates
- Total gate count
- Logic depth
- Functional equivalence before and after simplification

## 7. Expected Results

The eight Boolean functions should be implemented successfully. Their outputs should match the theoretical truth tables for all input combinations.

Equation 1
<img width="319" height="210" alt="Screenshot 2026-10-31 201851" src="https://github.com/user-attachments/assets/7db194af-7673-4b85-bd91-a29957c2ab56" />

Equation 2
<img width="306" height="179" alt="Screenshot 2026-10-31 202422" src="https://github.com/user-attachments/assets/1f63bbe6-fca5-4a47-8583-932db2f71c26" />

Equation 3
<img width="224" height="122" alt="Screenshot 2026-10-31 203110" src="https://github.com/user-attachments/assets/39e6cd8b-ce9a-4608-b568-b4c5e5081494" />

Equation 4
<img width="455" height="316" alt="Screenshot 2026-10-31 204422" src="https://github.com/user-attachments/assets/dcff3247-edab-4a98-b583-ad9f713e6112" />

Equation 5
<img width="405" height="373" alt="Screenshot 2026-10-31 210158" src="https://github.com/user-attachments/assets/241f0eea-3085-416d-ad43-baf9ab001eef" />

Equation 6
<img width="400" height="305" alt="Screenshot 2026-10-31 211332" src="https://github.com/user-attachments/assets/3c105282-d251-4948-a8e7-629a7d53f780" />


Equation 7
<img width="396" height="293" alt="Screenshot 2026-10-31 205621" src="https://github.com/user-attachments/assets/48a4f56e-babe-43fd-826d-c1dfd822ab61" />


Equation 8
<img width="397" height="307" alt="Screenshot 2026-10-31 212052" src="https://github.com/user-attachments/assets/ddd6a6b6-71d3-40b4-90a4-bd8652be40eb" />


## 8. Result

The logic circuits are designed, implemented, and verified using Boolean algebra and digital logic gates. The original and simplified circuits are compared based on gate count and logic depth.

## 9. Repository Structure

```text
EXPERIMENT-01-BUILDING-LOGICAL-CIRCUITS/
├── README.md
├── circuit_diagrams/
├── truth_tables/
├── simulation_files/
└── results/
```

## 10. Viva Questions

1. What are universal logic gates?
2. State De Morgan's theorems.
3. What is the difference between SOP and POS?
4. How does XOR differ from XNOR?
5. How can Boolean expressions be simplified?
6. How many truth-table rows are required for six inputs?
7. What is logic depth?
8. Why is functional verification necessary?
