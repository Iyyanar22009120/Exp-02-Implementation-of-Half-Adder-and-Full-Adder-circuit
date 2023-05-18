# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: mathan raj
RegisterNumber: 212222230079
```
## HALF ADDER
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
## FULL ADDER
```
module full_adder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
### Output:
## Logic symbol & Truthtable
## HALF ADDER
![3 half](https://user-images.githubusercontent.com/118680259/233821052-11a02f36-7b28-4be0-86b1-3b1229aea230.png)
## FULL ADDER
![3 full](https://user-images.githubusercontent.com/118680259/233821060-b5f93657-c770-4ba1-b3c7-8d7458827c73.png)

## RTL realization
## HALF ADDER
![3 rtl half](https://user-images.githubusercontent.com/118680259/233821094-bde94414-1deb-4b3e-8afe-a45ac1c275d0.png)
## FULL ADDER
![3 rtl full](https://user-images.githubusercontent.com/118680259/233821215-4eeea36c-6e4e-43a8-93ec-bda95ee3f7e6.png)


### RTL
### TIMING DIAGRAM
## HALF ADDER
![timing half](https://user-images.githubusercontent.com/118680259/233821221-84041234-2591-4fb6-8cfd-a1a5579c5f4a.png)
## FULL ADDER
![timing full](https://user-images.githubusercontent.com/118680259/233821230-720ea32f-6f16-4bbb-8f4d-8ac8aa95241f.png)
### Result:
Thus,the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
