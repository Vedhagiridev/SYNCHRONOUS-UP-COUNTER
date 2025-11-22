### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

Program for flipflops and verify its truth table in quartus using Verilog programming. 
<img width="829" height="437" alt="Screenshot 2025-11-22 201527" src="https://github.com/user-attachments/assets/435cc5be-ac25-4aa8-bd2c-8682e7529c73" />

Developed by:SHARMILI.V RegisterNumber:25011856
**RTL LOGIC UP COUNTER**
<img width="1117" height="359" alt="Screenshot 2025-11-22 201542" src="https://github.com/user-attachments/assets/1baaa01c-f2a4-4eb3-a0d7-0e8fb42c1b11" />

**TIMING DIAGRAM FOR IP COUNTER**
**TRUTH TABLE**
<img width="1130" height="148" alt="Screenshot 2025-11-22 201558" src="https://github.com/user-attachments/assets/f1817025-171e-40a4-8f94-37c718377801" />

**RESULTS**
Thus, implement 4 bit synchronous up counter and validate functionality.
