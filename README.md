# BOOLEAN_FUNCTION_MINIMIZATION
NAME:SATHISH.B

REG NO:24900077


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
```
module booleanfunction(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign x6=(~w)&(~x)&(~y)&(~z);
assign x7=(w)&(~y)&(~z);
assign x8=(~x)&(y)&(~z);
assign x9=(~w)&(x)&(y)&(z);
assign x10=(x)&(~y)&(z);
assign f1=x1|x2|x3|x4|x5;
assign f2=x6|x7|x8|x9|x10;
endmodule 

Developed by: RegisterNumber:*/

```
**TRUTH TABLE**
![exp2 tt](https://github.com/user-attachments/assets/66cc74dc-5c40-4d41-b2ed-236923f4550a)


**Output:**
![exp2 wave](https://github.com/user-attachments/assets/05144057-b3e2-4c65-825b-e56666e0e08f)

**RTL**

![exp2](https://github.com/user-attachments/assets/d8a5e0ac-d83d-493f-a8fa-4cde6f8e1420)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

