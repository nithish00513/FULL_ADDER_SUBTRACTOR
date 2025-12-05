# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**
*Half_adder*
module halfadd_top(a,b,sum,carry);
input a,b;
output sum,carry; 
 assign sum = a^b;
 assign carry = a & b;
endmodule

*Half_subtractor*
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo; // Outputs sum and carry for half adder:Outputs difference D,Borrow Bo for half subtractor
assign D = a ^ b;
  assign Bo = ~a & b;
endmodule


/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 

Developed by: Nithish Kumar S 

RegisterNumber: 212224230190
*/

**RTL Schematic**
FULL ADDER
<img width="1918" height="1078" alt="EXP04 FULL ADDER " src="https://github.com/user-attachments/assets/cbf834c8-6767-4c3c-b9f4-daf94e0ed4a8" />
FUll SUBTRACTOR
<img width="1918" height="1078" alt="EXP4 FULL SUBTRACTOR" src="https://github.com/user-attachments/assets/314bb1c2-0cfa-49e2-b62d-c5caac31c498" />

**Output Timing Waveform**
FULL ADDER
<img width="1918" height="1078" alt="EXP04 FULL ADDER clock diagram" src="https://github.com/user-attachments/assets/008039ae-76b4-4524-ac6f-7300ed36bf16" />
FULL SUBTRACTOR 
<img width="1918" height="1078" alt="EXP4 FULL SUBTRACTOR CLOCK DIAGRAM" src="https://github.com/user-attachments/assets/57c51778-8eae-4090-9ff7-198e48617d5d" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



