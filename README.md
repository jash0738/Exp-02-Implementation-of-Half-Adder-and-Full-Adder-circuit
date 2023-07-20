# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
*/
Logic symbol & Truthtable
RTL realization
### Output:
### RTL (HALF ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/25c8b5e2-c560-403f-977c-47200cec6d9d)
### TIMING DIAGRAM (HALF ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/952c6177-9fb4-4893-b4b2-2c920ade1376)
### TRUTH TABLE (HALF ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/b29b1018-f608-404d-a7a1-340d6cad6d32)
### RTL (FULL ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/8750105a-67cf-4c0d-9f95-4dc9236a9335)

### TIMING DIAGRAM (FULL ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/a355d9ca-85bf-48eb-b7f9-1021b9cf234b)

### TRUTH TABLE  (FULL ADDER )
![image](https://github.com/jash0738/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841600/8e4ccd7d-c1a5-4ce6-9d62-baf7a3b84373)

### Result:
