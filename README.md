# BOOLEAN_FUNCTION_MINIMIZATION
## DEVELOPED BY: Vikamuhan.N
## REGISTRATION NUMBER : 212223240181

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

```
module ex2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization:
![image](https://github.com/vikamuhan-reddy/BOOLEAN_FUNCTION_MINIMIZATION/assets/144928933/4260a4a4-1ce7-47f0-b0ff-4d36244a4c19)

## TRUTHTABLE:
![image](https://github.com/vikamuhan-reddy/BOOLEAN_FUNCTION_MINIMIZATION/assets/144928933/078165ec-23e4-47fa-a113-7494071568fa)


## Timing Diagram:
![image](https://github.com/vikamuhan-reddy/BOOLEAN_FUNCTION_MINIMIZATION/assets/144928933/c3b12af4-ac75-4fc2-ac30-6178f600536d)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

