# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of reducing a Boolean expression to its simplest form.
It removes unnecessary terms and variables to create an efficient logic circuit.
The minimized form uses fewer gates, reducing cost and power.
Methods include algebraic simplification, K-Maps, and the Quine–McCluskey method.

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(w&y)|(x&y));
endmodule

```

**Output:**

**RTL realization**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/48e50544-d70d-47d9-b73e-6356008a8a89" />


**RTL**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b56c49cb-9db8-44bd-8167-788f1ebdf118" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

