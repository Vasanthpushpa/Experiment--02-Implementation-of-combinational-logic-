# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:

/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: VASANTH P
RegisterNumber:  212222240113
*/
```
module cpmbine(a,b,c,d,f);
input a,b,c,d;
output f;
wire p,q,r;
assign p=(~c & b & a);
assign q=(~d & c & c & a);
assign r=(c & ~b & a);
assign f=(~(~p & ~q & ~r));
endmodule

module combine1(a,b,c,d,f);
input a,b,c,d;
output f;
wire p,q,r;
assign p=(c & ~b & a);
assign q=(d & ~c & a);
assign r=(c & ~b & a);
assign f=((p | q & |r));
endmodule
```
## RTL realization

## Output:
## RTL
![image](https://user-images.githubusercontent.com/119291100/234768357-f4cd4d68-6d09-4113-a116-cdc9b1ac2b34.png)
![image](https://user-images.githubusercontent.com/119291100/234768392-015f2c62-3049-4a25-a5e6-c3e96f24d4fc.png)


## Timing Diagram
![image](https://user-images.githubusercontent.com/119291100/234768432-0d96815d-ac4f-44fe-868a-42f482f5ddc6.png)
![image](https://user-images.githubusercontent.com/119291100/234768453-6a3ccda1-658a-4dfd-b157-30ca4d69bbd6.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
