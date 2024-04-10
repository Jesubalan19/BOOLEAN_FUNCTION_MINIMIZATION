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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Jesubalan A
RegisterNumber: 212223240060
*/
```
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
**RTL realization**

**Output:**
![dig 0](https://github.com/Jesubalan19/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979294/fa22a4fb-8627-4605-9544-28f521ca5b39)

**RTL**
![dig 1](https://github.com/Jesubalan19/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979294/02dece33-9339-4a9f-905d-307ec828877c)

**Timing Diagram**
![dig 2](https://github.com/Jesubalan19/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979294/c845fbd4-5965-490e-87fe-621b37f73b3f)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

