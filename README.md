***NAME : RAMYA G***


REGISTER NO : 212224220078

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

![Screenshot 2025-03-19 035947](https://github.com/user-attachments/assets/b8f35b29-aa66-4221-a177-a57d94467eb8)


**Procedure**

Write the detailed procedure here

**Program:**
```
module ex4(a,b,c,sum,carry,difference,borrow);
input a,b,c;
output sum,carry,difference,borrow;
assign sum=(a^b^c); 
assign carry= (a & b|a & c|b & c);
assign difference= (a^b^c);
assign borrow= (~a&b|~a&c|b&c);
endmodule


```
/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**

![Screenshot 2025-03-19 035650](https://github.com/user-attachments/assets/8c82f6ca-2492-4f1e-9b5f-5648dc33df4d)


**Output Timing Waveform**

![Screenshot 2025-03-19 024926](https://github.com/user-attachments/assets/9b663bff-4bb7-4e9e-b4cb-63454f4f03c7)


**Result:**

Thus the given Full-Adder-And-Full-Subtractor circuits are verified successfully  in QUATRUS II by verilog HDL programming.



