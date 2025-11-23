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
<img width="1600" height="879" alt="image" src="https://github.com/user-attachments/assets/ebb9374c-ef2a-44e7-84e8-999ad43b2a7c" />

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**Program:**

 Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
 Developed by: RegisterNumber:25017133
```
module exp4(a,b,c,s,C);
input a,b,c;
output s,C;
assign s=a^b^c;
assign C=(b&c)|(a&c)|(a&b);
endmodule

module exp4(a1,b2,c3,d,B);
input a1,b2,c3;
output d,B;
assign d=a1^b2^c3;
assign B=(~a1&c3)|(b2&c3)|(~a1&b2);
endmodule

```

**RTL Schematic**
**Full_adder**

<img width="651" height="459" alt="image" src="https://github.com/user-attachments/assets/89a7b8b6-81bc-460b-9408-fd75a3873cca" />

**Full_subtractor**

<img width="1048" height="595" alt="image" src="https://github.com/user-attachments/assets/2ab8686f-2a05-4e5e-ad20-b02f97873f48" />

**Output Timing Waveform**

**Full_adder**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ad716dfc-2bbc-43c1-b67a-70ab216d2a55" />

**Full_subtractor**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/da921813-0cfa-4916-826f-d38a7236f374" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



