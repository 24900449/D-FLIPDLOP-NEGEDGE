# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**

/* write all the steps invloved */ 1.Open quartus II and create New project wizard. 2. Write the program in Verilog HDL file and run the program. 3. Download the RTL viewer 4. Now open university program VWF and download waveform after the execution.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 
 module Exp8(D,clk,Q,Qbar); input D,clk; output reg Q; output reg Qbar; initial Q=0; initial Qbar=1; always @(posedge clk) begin Q=D; Qbar=~D; end endmodule
**RTL LOGIC FOR FLIPFLOPS**

![389434778-88c27dd5-f50f-4c78-b59b-3fe0a2aabed7](https://github.com/user-attachments/assets/08da0b0f-e46e-4574-9a87-07b7baf7e2c2)


**TIMING DIGRAMS FOR FLIP FLOPS**

![389434863-3941f68b-040d-446f-9322-b468127b81f8](https://github.com/user-attachments/assets/ac2e3d4e-dc24-45c0-8ead-d6cea5dc988a)


**RESULTS**Thus the D flip flop is executed in Verilog and the output is verified.
