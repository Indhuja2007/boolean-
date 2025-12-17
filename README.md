# boolean
AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

Logic Diagram

Screenshot 2025-11-20 185008
Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program: Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
Developed by:BALAJI T RegisterNumber:25005672

RTL realization Screenshot (31)

Output:

RTL Timing Diagram Screenshot (32)

Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
