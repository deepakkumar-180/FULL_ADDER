# FULL_ADDER
Implementation-of-Full-Adder-circuit

AIM:

To design a Full Adder circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

 ``` Hardware – PCs, Cyclone II , USB flasher ```
Software – Quartus prime

Full Adder:

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin

Carry = AB + ACin + BCin

Program:
```
module Full_adder(
    input  wire a, b, cin,   
    output wire sum, carry   
);

    
    assign sum   = a ^ b ^ cin;              
    assign carry = (a & b) | (b & cin) | (a & cin); 

endmodule
```
NAME : DEEOAKKUMAR S REF NO: 25016457

RTL Schematic [image.pdf](https://github.com/user-attachments/files/24143310/image.pdf)




Output Timing Waveform [wave4.pdf](https://github.com/user-attachments/files/24143311/wave4.pdf)


Result: Thus the Full Adder circuits are designed and the truth tables is verified using Quartus software.
