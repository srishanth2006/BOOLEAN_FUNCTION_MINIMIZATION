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
module boolean_minimization(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
```

# Developed by: SRISHANTH J
# RegisterNumber:212223240160



# TRUTH TABLE
<img width="639" alt="image" src="https://github.com/user-attachments/assets/1112e448-5c42-411f-ab66-09ec3645c5a4">
   
   
<img width="635" alt="image" src="https://github.com/user-attachments/assets/a9c14a1c-ca01-45c7-b404-97dbe87adc85">


**RTL**


<img width="538" alt="image" src="https://github.com/user-attachments/assets/d177884d-d006-48be-b4c6-f93be71480a1">

**Output:**


<img width="487" alt="image" src="https://github.com/user-attachments/assets/a9170a7c-24df-4be8-9eb7-b00dd5f610d5">



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

