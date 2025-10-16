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


<img width="501" height="533" alt="image" src="https://github.com/user-attachments/assets/6dc08a4f-305c-43b1-9c7b-881340887ef6" />


<img width="639" height="590" alt="image" src="https://github.com/user-attachments/assets/bafd5fc9-83cb-419a-9eef-9b4cdbfd9e46" />



**Procedure**
 Full Adder: 1.Open Quartus II and create a new project. 2.Use schematic design entry to draw the full adder circuit. 3.The circuit
 consists of XOR, AND, and OR gates. 4.Compile the design, verify its functionality through simulation. 5.Implement the design on the
 target device and program it.
 3/4
 https://github.com/mahith777/FULL_ADDER_SUBTRACTOR/blob/main/README.md
Full Subtractor: 1.Follow the same steps as for the full adder. 2.Draw the full subtractor circuit using schematic design. 3.The circuit
 includes XOR, AND, OR gates to perform subtraction. 4.Compile, simulate, implement, and program the design similarly to the full
 adder

Write the detailed procedure here

**Program:**
module FAHA1 (a,b,c,x,y,z,sum,dif,car,bor); input a,b,c,x,y,z; output sum,dif,car,bor; assign sum = a^b^c; assign car = a&b |
 a&c | b&c; assign dif = x^y^z; assign bor = ~x&z | ~x&y | y&z; endmodule

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:Shafi Ahmed MS RegisterNumber:25014933
*/

**RTL Schematic**

<img width="503" height="415" alt="image" src="https://github.com/user-attachments/assets/ce98d894-2881-4e39-b9d8-9364af347984" />


**Output Timing Waveform**

<img width="821" height="166" alt="image" src="https://github.com/user-attachments/assets/0af1af5a-f6bf-4e9f-9b58-5a2ffb984361" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



