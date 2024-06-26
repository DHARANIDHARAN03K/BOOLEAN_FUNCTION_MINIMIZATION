# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


Program:

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: DHARANI DHARAN K
RegisterNumber:212223040036
```
module ex02(A,B,C,D,F1);

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


RTL realization


Output:

![image](https://github.com/DHARANIDHARAN03K/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870858/dc2252ac-df19-487d-a54d-978071c37196)


Truth table:

![image](https://github.com/DHARANIDHARAN03K/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870858/64136d91-6616-4c51-b9f7-f9f7f3a05e95)



RTL

Timing Diagram

![image](https://github.com/DHARANIDHARAN03K/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870858/d7edc05e-2822-4822-bea7-528ebcf96817)


Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

