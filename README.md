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

1.Open Quartus and create a new project.

2.Create a Verilog HDL file and type the 4-bit ripple counter code.

3.Save the file and set it as Top-Level Entity.

4.Compile the program using Processing → Start Compilation.

5.Create a Waveform File (VWF) and insert input/output nodes (clk, q[3..0]).

6.Apply clock input to clk using Value → Clock.

7.Run Functional Simulation.

8.Observe the output waveform and verify the counter sequence from 0000 to 1111.

~~~
 Developed by: Arunachalam M
 RegisterNumber: 212225230019
~~~

**PROGRAM**

 Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming
 
~~~
 module digital9(out,clk,rst); 
 input clk,rst; 
 output reg [3:0]out; 
 always @ (posedge clk)
 begin 
 if(rst) 
 out<=0; 
 else 
 out <= out-1; 
 end endmodule
~~~

**RTL LOGIC FOR 4 Bit Ripple Counter**

<img width="1037" height="538" alt="rtf" src="https://github.com/user-attachments/assets/58fcc2ce-6a7c-43d7-ad9a-80083e95d964" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="1275" height="677" alt="op" src="https://github.com/user-attachments/assets/d7e35bf1-9d3b-47e0-8888-21fda060c8cf" />

**RESULTS**
Thus, To implement 4 Bit Ripple Counter using verilog and validating their functionaly using their functional tables is executed succsessfully.
