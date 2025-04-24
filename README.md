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
module exp2(A,B,C,D,W,X,Y,Z,F1,F2);
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
assign F1=(~B)&(~D)|(A)&(B)&(~C)|(~A)&(B)&(D);
assign F2=(~X)&(Z)|(X)&(Y)|(W)&(Y);
endmodule
```


Developed by:Gowtham S RegisterNumber:212224100018


**RTL realization**

**Output:**
![WhatsApp Image 2025-04-24 at 10 55 12_36f99db9](https://github.com/user-attachments/assets/cbea353e-cbaf-43e0-b8c5-19fec3aca0de)


**RTL**
![WhatsApp Image 2025-04-24 at 11 12 55_15e24bdc](https://github.com/user-attachments/assets/011eb2ee-efda-495c-bad7-144c2d5ed549)


**Timing Diagram**
![WhatsApp Image 2025-04-24 at 11 12 54_fb8020f9](https://github.com/user-attachments/assets/a4864944-83f5-476d-ad5f-937e2bf3ef10)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

