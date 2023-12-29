## Developed by: Farhana H
## Register number:212223230057
# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 F2=xy’z+x’y’z+w’xy+wx’y+wxy
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime
## Theory:
  combinational Logic Circuits are memoryless digital logic circuits whose output at any instant in time depends only on the combination of its inputs.The outputs of combinational Logic Circuits are only determined by the logical function of their current input state,logic "0" or logic "1",at any given instant in time.
  The result is that combinational logic circuits have no feedback,and any changes to the signals being applied to their inputs will immediately have an effect at the output.In other words,in aCombinational Logic Circuits,yhe output is dependent at all times on the combination of its inputs.Thus,a combinational circuit is memoryless.
 ## Procedure:
 ```
 1.Type the program in Quartus software.
 2.Compile and run the program.
 3.Generate the RTL schematic and save the logic diagram.
 4.Create the nodes for inputs and outputs to generate the timing diagram.
 5.For the different input combination,generate the timing diagram.
```
## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Farhana H
RegisterNumber: 212223230057
module ex_02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule

/*
```
## RTL realization

![image](https://github.com/syedfayaz3105/Experiment--02-Implementation-of-combinational-logic-/assets/147144126/113782ee-8e61-444e-9014-72ab557600ef)
## Truth table:
![image](https://github.com/syedfayaz3105/Experiment--02-Implementation-of-combinational-logic-/assets/147144126/9a8554de-8285-419d-b1c4-7fc60f1d1701)
## Output:
![image](https://github.com/syedfayaz3105/Experiment--02-Implementation-of-combinational-logic-/assets/147144126/a0aba158-3371-45cb-a0ce-649ec951e300)
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
