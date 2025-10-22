# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

# AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

# Half Subtractor:

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

# Truthtable

# Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


# Program:

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
module ha(a,b,sum,carry); 
input a,b; 
output sum,carry; 
assign sum= (a ^ b); 
assign carry= ( a & b); 
endmodule
```
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
ii)HALF SUBTRACTOR
```
module hs(a,b,difference,borrow); 
input a,b; 
output difference,borrow; 
assign difference= (a ^ b); 
assign borrow= ( ~a & b); 
endmodule


Developed by:Kavya G  RegisterNumber:25018973
```
Developed by: sanjay srisanth RegisterNumber:25018855

# RTL Schematic
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/8a2130ef-793f-4dc4-afe8-48d071b1209f" />
<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/162c943a-f7ed-434c-9226-374533360283" />

**Output/TIMING Waveform**
<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/4d3ae9ea-8968-436b-bd8b-131f49d6f744" />
<img width="1920" height="1020" alt="4" src="https://github.com/user-attachments/assets/a1d931af-8e2a-4a75-8637-c20e689e5615" />

## Result:
Thus the half adder and half subtractor are designed and the truth tables is verified using quartus software.
