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
Developed by: LOKESHVARAN S
RegisterNumber:  23012889
*/
## Program:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: THAMARAISELVAN V
RegisterNumber:  212221230115


Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
## Output:
## RTL
Half adder:
![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/7b31d0d3-e505-417d-b9c9-059b032fa11b)
Full adder:

![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/f03a0182-9abf-43cc-8133-69b912c51671)
## TIMING DIAGRAM:
Half adder

![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/a502b958-f78a-420d-9fa4-26b27dabdc89)
Full adder

![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/6598f104-34ee-4079-9a93-70a8b888be8e)
## TRUTH TABLE
Half adder
![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/2585d5f0-7584-4d09-9cc4-285691b44610)
Full adder
![image](https://github.com/Lokeshvaran9600/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145972263/ccbda33b-cf47-4c3b-a80d-41108b450694)
Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
