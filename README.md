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
Developed by:SRISHANTH J
RegisterNumber:212223240160
```
```
module de_exp_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule
```
```
module proj23(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```

**Truth Table:**

*F1*

<img width="454" alt="image" src="https://github.com/user-attachments/assets/44ad7cff-a7ae-4704-908e-5ef376695167">


*F2*

<img width="440" alt="image" src="https://github.com/user-attachments/assets/c8b3fd63-d569-47bc-9801-586c203c766f">


**RTL:**

*F1*
<img width="563" alt="image" src="https://github.com/user-attachments/assets/35df52ae-e551-47a6-b4aa-c292e842f7e3">

*F2*
<img width="417" alt="image" src="https://github.com/user-attachments/assets/91c59730-4bf1-4b6b-9769-2fafcc969450">



**Timing Diagram:**

*F1*
<img width="567" alt="image" src="https://github.com/user-attachments/assets/0f7c5112-c120-4e11-9963-67b912334f69">

*F2*
<img width="566" alt="image" src="https://github.com/user-attachments/assets/ca81a8a4-a980-4a5a-a793-ccd0477aaed3">


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

