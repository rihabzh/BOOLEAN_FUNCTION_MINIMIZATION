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

1. module ex2 (a,b,c,d,w,x,y,z,f1,f2);
2. input a,b,c,d,w,x,y,z;
3. output f1,f2;
4. assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
5. assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
6. endmodule

Developed by:RIHAB ZAKKAIR HUSSAIN
RegisterNumber:25015140 */


**RTL realization**
<img width="740" height="813" alt="ex2" src="https://github.com/user-attachments/assets/6e3e43ec-6924-4061-bdba-7d356f3bd9f1" />

**Output:**
<img width="1918" height="398" alt="ex2 1" src="https://github.com/user-attachments/assets/54d5b5d2-99f0-4cc8-816a-bbbd27be3f58" />

**RTL**

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

