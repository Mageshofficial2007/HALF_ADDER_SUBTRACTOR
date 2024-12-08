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
1) HALF ADDER
 
![WhatsApp Image 2024-12-08 at 19 33 49_2233cca9](https://github.com/user-attachments/assets/ba84058b-739f-40bf-bc46-54164fcc219f)

2) HALF SUBRACTOR

![WhatsApp Image 2024-12-08 at 19 34 51_9c930fc5](https://github.com/user-attachments/assets/4cf1ce27-2cfc-4f79-804f-bbcf4bba3e78)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

1)HALF ADDEER
```
module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule
```
2) HALF SUBRACTOR
```
module halfsubractor(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule
```
Developed by: MAGESH BOOPATHI.M

RegisterNumber:24900855
*/

**RTL Schematic**
1) HALF ADDEER

![391319522-ae607d99-b8b8-4135-bb16-164b816109a6](https://github.com/user-attachments/assets/5ea7839f-7a7f-4fe4-bad0-f4b140c7c5f0)


2) HALF SUBRACTOR

 ![391319543-92a0eff7-49b1-4e8b-a65c-aaaaa3885c40](https://github.com/user-attachments/assets/c20cc008-f390-4284-998a-0379895a8d7f)



**Output/TIMING Waveform**

1) HALF ADDEER

![WhatsApp Image 2024-12-08 at 19 57 43_9b6b61bb](https://github.com/user-attachments/assets/f7637fac-61df-4259-a8ce-15dc6d1fe30a)



2) HALF SUBRACTOR

![WhatsApp Image 2024-12-08 at 19 57 47_f536911a](https://github.com/user-attachments/assets/0d627c21-3da9-4350-bf9d-f5bb97a409e7)



**Result:**

Thus the half adder and half subtractor circuit is designed and verified its truth table in Quartus using Verilog programming.
