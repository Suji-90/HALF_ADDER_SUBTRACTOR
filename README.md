### REGISTER NUMBER:212223040212
### NAME:SUJITHRA.K
# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

## AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

## Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

## Half Subtractor

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

## Truthtable
![319871508-57dc5dce-68c2-4313-8a7d-fcdcb80f5c10](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/150884148/2dcae032-fc0a-4bed-8f91-d5334a68d9e8)

## Procedure

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

## Half Adder
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry; 
assign sum = a^b;
assign carry = a & b;
endmodule
```
## Half Subtractor
```
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo; 
assign D = a ^ b;
assign Bo = ~a & b;
endmodule
```
## RTL Schematic
![319870809-c62bec9f-dad1-44e1-a264-2c9c6ed4b0f3](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/150884148/8f47a414-ca6c-4f36-98f3-1063d242a103)


## Output/TIMING Waveform
## Half_adder
![319871027-90070605-88a0-4425-8171-255445aacb74](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/150884148/3c2d2a54-58c6-4fe0-9568-4f793b6dc621)

## Half_subtractor
![319871129-c3ea5705-438a-484f-9199-6e3bcff60482](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/150884148/58dd5759-7f12-49b9-818c-79bc2d957166)

## Result:
Thus the given Half adder subtractor are verified using verilog programming
