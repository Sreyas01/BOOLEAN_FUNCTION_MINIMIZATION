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
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

Developed by:Sreyas RegisterNumber:24004091

**TRUTH TABLE**
![389950015-386b7362-5711-4a02-9096-500396ec4acf](https://github.com/user-attachments/assets/dd39e87c-4466-4801-a4e1-46dd9a95e0a3)

![389950122-d60ded4e-5d58-423e-a8a8-cfaf86fecf69](https://github.com/user-attachments/assets/2309d610-3bcd-4b71-8866-e50823eeec46)


**RTL realization**
![image](https://github.com/user-attachments/assets/6efcd6a4-5fc2-4cb3-9544-d79d258159f5)


**Output Waveform:**
![389944365-f04a1f0d-c022-4844-8bfb-4c885a5b736c](https://github.com/user-attachments/assets/9a894ea1-96db-48be-893d-540b6f78c1c6)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

