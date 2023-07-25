# Exp-03 Implementation of HalfAdder and Full Adder circuit

# Implementation of Half Adder and Full Adder circuit
### name: Jashwanth M.R   
### reg no: 23005691
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder:
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder:
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

## Procedure:-
1. Create a New Project:
   - Open Quartus and create a new project by selecting "File" > "New Project Wizard."
   - Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

2. Create a New Design File:
   - Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
   - Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

3. Write the Combinational Logic Code:
   - Open the newly created Verilog or VHDL file and write the code for your combinational logic.
     
4. Compile the Project:
   - To compile the project, click on "Processing" > "Start Compilation" in the menu.
   - Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5. Analyze and Fix Errors:*
   - If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
   - Review and fix any issues in your code if necessary.
   - View the RTL diagram.

6.*Verification:
   - Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
   - Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
   - Give the Input Combinations according to the Truth Table amd then simulate the Output Waveform.
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
Thus the given logic function is implemented using and or and not gate and their operations are verified using Verilog programming.
