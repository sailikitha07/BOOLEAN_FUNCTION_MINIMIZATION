![Screenshot 2024-11-27 231427](https://github.com/user-attachments/assets/a96085e2-6c33-4519-96d8-d4369b733784)# BOOLEAN_FUNCTION_MINIMIZATION

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

Developed by:sai likitha  RegisterNumber:24009865
module exp07(A, B, C, D, W, X, Y, Z, F1, F2);
input A, B, C, D, W, X,Y,Z;
wire x1, x2, x3, x4, x5, x6, x7, x8, x9, x10;
output F1, F2;
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
endmodule */

```

**RTL realization**
![Screenshot 2024-11-27 225856](https://github.com/user-attachments/assets/468373d4-24f3-4752-85a9-3ad6e2f63608)

**Output:**
![Screenshot 2024-11-27 233707](https://github.com/user-attachments/assets/ce9e49db-305a-4c79-942e-c9f0985c9325)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

