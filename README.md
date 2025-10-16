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

Developed by: JACK WALLACE */
i) module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
ii) module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


**RTL realization**

<img width="712" height="790" alt="image" src="https://github.com/user-attachments/assets/aab74cf6-631f-4ce1-8117-88144bef635c" />

**Output:**

**RTL**

**Timing Diagram**

F1:

<img width="1755" height="327" alt="image" src="https://github.com/user-attachments/assets/36401d84-7bfe-49f6-8ba5-b22ef15b2a21" />

F2:

<img width="1750" height="394" alt="image" src="https://github.com/user-attachments/assets/508b3dad-85bc-495a-8a60-6e67181cc243" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

