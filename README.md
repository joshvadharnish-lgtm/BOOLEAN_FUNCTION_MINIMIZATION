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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```
 

Developed by: G.DHARNISH  RegisterNumber:21225040069


**RTL realization**
<img width="1917" height="1013" alt="image" src="https://github.com/user-attachments/assets/16ec4ea8-7e20-42f0-acf0-aa8d9f828748" />


**Output:****RTL**
<img width="1917" height="1013" alt="image" src="https://github.com/user-attachments/assets/364bd135-8010-49a3-af61-228fa17fc09d" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

