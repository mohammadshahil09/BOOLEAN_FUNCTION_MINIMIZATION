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
Program to implement the given logic function and
to verify its operations in quartus using Verilog programming. 

Developed by: Guntur shaik mohammad shahil
RegisterNumber: 212223240044

module combinationalcircuit(A,B,C,D,F1);
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


**RTL realization:**

![Screenshot 2024-03-20 162908](https://github.com/mohammadshahil09/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742840/fe6a7ceb-4fd3-4daf-b2fe-65d12be2eabc)


**Truth Table:**

![Screenshot 2024-03-20 162929](https://github.com/mohammadshahil09/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742840/dfce9909-dbec-4cb9-9a51-763435856651)


**Timing Diagram:**

![Screenshot 2024-03-20 162943](https://github.com/mohammadshahil09/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742840/d71f69fb-b68c-476f-b699-300c37e57b0b)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

