### NAME: DIVYA K
### REG NO:212222230035

# Exp 03 Implementation of Half Adder and Full Adder circuit

# Implementation of Half Adder and Full Adder circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin
#### HALF ADDER 

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

####  FULL ADDER 

![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)


### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:

### Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
Developed by: DIVYA K
RegisterNumber:  212222230035
```
```
module EX03(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
```
```
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```
*/
Logic symbol & Truthtable



### RTL DIAGRAM
### HALF ADDER
![Screenshot 2023-09-01 083932](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/ca76c4d2-ee1a-4d08-bcff-58c1436fd4c2)
### FULL ADDER
![image](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/c52a0292-10d3-4202-a37d-8475debf3300)


### OUTPUT WAVEFORM

### HALF ADDER
![WhatsApp Image 2023-09-01 at 09 39 10](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/c41a348e-bb24-4dd1-905c-275d8e092117)

### FULL ADDER
![image](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/146dc2b7-4bae-4816-b671-67ead4d3fe26)


### TRUTH TABLE 
### HALF ADDER
![image](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/5a94cfcd-4578-4dc1-b309-54a530ecb635)

### FULL ADDER
![image](https://github.com/divyakumars/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393621/d4c15c60-30e9-47d2-8ba1-43d52689ca22)


### Result:
Thus the Implementation of Halfadder Fulladder Circuit are studied and the truthtable for different logic gates are verified
