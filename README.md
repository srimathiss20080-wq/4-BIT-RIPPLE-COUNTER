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

/* write all the steps invloved */

**PROGRAM**
```
module ripple_counter_4bit (
    input wire clk,
    input wire rst,
    output reg [3:0] q
);
    always @(posedge clk or posedge reset) begin
        if (reset)
            q <= 4'b0000;
        else
            q <= q+ 1'b1;         // increments like a ripple counter
    end

endmodule
```

 Developed by: SRIMATHI S
 RegisterNumber: 25017525

**RTL LOGIC FOR 4 Bit Ripple Counter**


<img width="1064" height="408" alt="Screenshot 2025-12-13 164343" src="https://github.com/user-attachments/assets/d7762b13-fa49-4293-9d46-eada3841f8b0" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="1062" height="158" alt="Screenshot 2025-12-13 164354" src="https://github.com/user-attachments/assets/ad070744-25ef-4726-a6f7-d2c331a4968f" />


**RESULTS**
Thus,implemented 4 Bit Ripple Counter using verilog and validating their functionality using their functional tables
