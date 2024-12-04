# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

i)HALF ADDER

<img width="563" alt="Screenshot 2024-11-29 at 7 50 14 PM" src="https://github.com/user-attachments/assets/00eb183d-8ba4-46e2-aff8-32464853c533">

ii)HALF SUBTRACTOR

<img width="291" alt="Screenshot 2024-11-29 at 7 40 07 PM" src="https://github.com/user-attachments/assets/19d14474-bd20-4841-af8a-c7f1b68170de">

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Program:**
```

i)HALF ADDER

module ha(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry





ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule





/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: V.Patrick Alex Emmanuel

RegisterNumber: 24900019
```
**RTL Schematic**

HALF ADDER

<img width="1470" alt="Screenshot 2024-11-29 at 11 12 14 PM" src="https://github.com/user-attachments/assets/0b8371c2-9719-41ac-b52d-95efe74d8302">

HALF SUBTRACTOR

<img width="1470" alt="Screenshot 2024-11-29 at 7 14 46 PM" src="https://github.com/user-attachments/assets/cb9f618c-7866-4d75-80a8-f42080a8fb90">

**Output/TIMING Waveform**

HALF ADDER

<img width="1464" alt="Screenshot 2024-11-29 at 11 03 36 PM" src="https://github.com/user-attachments/assets/431b377f-a53a-4554-9d7a-419cd4039a56">

HALF SUBTRACTOR

<img width="1466" alt="Screenshot 2024-11-29 at 11 07 30 PM" src="https://github.com/user-attachments/assets/eebb3469-ebe1-4a41-b7ef-0b0fc2c4d978">

**Result:**
Thus the Output's of encoder and decoder are verified by synthesizing and simulating the VERILOG code.
