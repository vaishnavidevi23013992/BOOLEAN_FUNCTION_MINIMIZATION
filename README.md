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


**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:VAISHNAVIDEVI V
RegisterNumber:212223040230
module (A,B,C,D,F1);
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



**RTL realization**


![2 1](https://github.com/vaishnavidevi23013992/BOOLEAN_FUNCTION_MINIMIZATION/assets/151864235/2a9ea591-788f-43e4-9ac2-72c55f6feec5)

**TRUTH TABLE**


![2 2](https://github.com/vaishnavidevi23013992/BOOLEAN_FUNCTION_MINIMIZATION/assets/151864235/ebce4c69-e09a-4b8b-b07b-cacddbd3a673)

**Timing Diagram**


![2 3](https://github.com/vaishnavidevi23013992/BOOLEAN_FUNCTION_MINIMIZATION/assets/151864235/b9312db6-f9e8-4754-bdcf-ce000b18f629)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

