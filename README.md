# README : Design and Simulation of 8-Bit Signed Arithmetic Unit.

## OVERVIEW

This repository / project package contains the resources, documentation, and simulation details for the academic project: **"
Design and Simulation of an 8-Bit Signed Arithmetic Unit
"**, developed for (DDCA) course.

This PPT explains the design and simulation of an 8-bit signed arithmetic unit for addition and subtraction.
It covers the circuit design, working process, Two’s Complement, and simulation testing.

---
## Slide Deck Overview(10 Slides)

=> **Slide 1 – Introduction**
   - Introduces the project, team members, department, and institution.

=> **Slide 2 – Problem & Abstract**
   - Explains why computers need to perform calculations with both positive and negative numbers and why this project is useful for learning digital design.

=> **Slide 3 – Objectives**
   - Describes what the project aims to do, including designing, building, testing, and checking the arithmetic unit.

=> **Slide 4 – Existing Systems**
   - Explains how this project is different from complex computer systems and how it provides a simple way to understand arithmetic circuits.

=> **Slide 5 – 8-Bit Arithmetic Unit**
   - Explains what an 8-bit system is, how signed numbers work, and how Two’s Complement is used for negative numbers.

=> **Slide 6 – System Design**
   - Shows the main parts of the system, including the input, control unit, ALU, and output.

=> **Slide 7 – Implementation**
   - Explains how the circuit is built using full adders, logic gates, multiplexers, and Two’s Complement.

=> **Slide 8 – Working Process**
   - Shows how the system takes two numbers, selects an operation, processes them, and produces the final result.

=> **Slide 9 – Testing**
   - Shows different addition and subtraction examples and confirms that the circuit gives the correct results.

=> **Slide 10 – Conclusion**
   - Summarizes what was achieved and learned, and mentions possible future improvements such as larger bit sizes and FPGA implementation.

---
## Logisim Simulation Setup Instructions
To run and verify the circuit in **Logisim**:

 1. **Requirement:**
    - Open Logisim or Logisim-evolution and create a new circuit.
    - Make sure the required logic gates and circuit components are available.
   
 2. **Building the 8-Bit Adder:**
    - Create two 8-bit input pins for numbers A and B.
    - Build a 1-bit Full Adder using XOR, AND, and OR gates.
    - Connect 8 Full Adders together to form the complete 8-bit adder.

3. **Adding Addition & Subtraction:**
   - Add a control switch to select Addition or Subtraction.
   - Use XOR gates to invert the bits of B during subtraction.
   - Add 1 to the inverted B value to perform Two’s Complement subtraction.
  
4. **Connecting the Output:**
   - Connect the 8-bit adder output to an 8-bit output pin or LEDs.
   - The output displays the final result of the selected operation.
  
5. **Testing and Verification:**
   - Test the circuit with different positive and negative values.
   - Check examples such as 5 + 3 = 8, 10 − 7 = 3, and 3 − 10 = −7.
   - Compare the Logisim output with the expected results to verify the circuit.

---

## Truth Table And Verification 

**For the 8-bit Signed Arithmetic Unit, you can use a simple verification matrix like this:**

| Test Case | A | B | Operation |  Expected Output | Status |
| :---: | :---: | :---: | :---: | :---: | :---: |
| `1` | `5` | `3` | `Addition` | `8` |**✓ Pass** |
| `2` | `-5` | `3` | `Addition` | `-2` | **✓ Pass** |
| `3` | `10` | `7` | `Subtraction` | `3` |**✓ Pass** |
| `4` | `15` | `-8` | `Addition` | `7` | **✓ Pass** |
| `5` | `3` | `10` | `Subtraction` | `-7` | **✓ Pass** |

**Verification:** The circuit is tested with both positive and negative numbers for addition and subtraction. The expected and actual outputs should match for every test case. These test cases are directly based on the verification results in your project.
