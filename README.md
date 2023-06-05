# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D F2=xy’z+x’y’z+w’xy+wx’y+wxy

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B

## Procedure:
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results

## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Thirukaalathessvarar S
RegisterNumber: 212222230161
*/
i.)
module exp2 (a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1 = (~b & ~d) | (~a &b & d) | (a & b & ~c);
endmodule

ii.)
module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2 = (x&y) | (y&w) | (`y&z);
endmodule
```
## RTL realization

## Output:
## RTL
1)For F1
![de_e2-o1](https://github.com/Thirukaalathessvarar-S/Experiment--02-Implementation-of-combinational-logic-/assets/121166390/3bf4ab7e-970e-4c62-b4ab-fc9e5922f0bc)
2)For F2
![def2(exp2)02](https://github.com/Thirukaalathessvarar-S/Experiment--02-Implementation-of-combinational-logic-/assets/121166390/b05c5bfd-58c2-4dc3-ba5a-aa3aa7236554)

## Timing Diagram
1)For F1
![def1(exp2)time (1)](https://github.com/Thirukaalathessvarar-S/Experiment--02-Implementation-of-combinational-logic-/assets/121166390/04c9d8c6-ca13-4531-9d3f-ba77feb7d96a)
2)For F2
![def2(exp2)time (1)2](https://github.com/Thirukaalathessvarar-S/Experiment--02-Implementation-of-combinational-logic-/assets/121166390/480fafdd-b287-40e0-a62f-a8884484be2c)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
