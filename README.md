# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

Type the program in Quartus software.
Compile and run the program.
Generate the RTL schematic and save the logic diagram.
Create nodes for inputs and outputs to generate the timing diagram.
For different input combinations generate the timing diagram./

**PROGRAM**
~~~
 module downcounter(out,clk,rst);
 input clk,rst;
 output reg [3:0]out;
 always @ (posedge clk)
 begin
    if(rst)
      out<=0;
    else 
      out <= out-1;
 end
 endmodule
~~~
Developed by: NANDHITHA S
RegisterNumber: 24900454


**RTL LOGIC FOR 4 Bit Ripple Counter**
![image](https://github.com/user-attachments/assets/bec01375-5de9-4d8a-a464-c16f2a9ca1da)

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
![image](https://github.com/user-attachments/assets/5d8b5559-a95e-40a2-895f-5d3cada123d5)

**RESULTS**
Thus, the Bit Ripple Counter is designed and its functionality is validated using the truth table and timing diagrams.
