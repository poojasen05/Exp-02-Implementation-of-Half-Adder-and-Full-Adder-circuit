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
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
Developed by:O.Sirisha Reddy
RegisterNumber:212222230103
*/

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
````
Truthtable:
half adder:

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/f8a33cf4-faec-4a3a-9a45-ba14ae1b5bda)

full adder:

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/abf97517-ea99-40f1-affd-438e68f6cadb)


RTL realization

half adder:

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/17b7b349-8cf3-4da8-91e7-6650fd7e733e)

full adder:

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/884932e9-6396-4dc5-ad8b-e1d0ef690b61)

Output waveform:

half adder

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/a204ccf6-66f1-43d4-ae24-b980509a1acc)

full adder

![image](https://github.com/Thenmozhi-Palanisamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/95198708/b5c9748a-da88-428a-9fda-90b04a98d9d0)


### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.


