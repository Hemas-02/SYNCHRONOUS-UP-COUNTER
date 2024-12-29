## SYNCHRONOUS-UP-COUNTER

## AIM:

To implement 4 bit synchronous up counter and validate functionality.

## SOFTWARE REQUIRED:

Quartus prime

## THEORY

## 4 bit synchronous UP Counter

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

## Procedure

/* write all the steps invloved */

## PROGRAM
![Screenshot 2024-12-29 150158](https://github.com/user-attachments/assets/62be725f-e23f-4d61-be69-bd79bfba1c6f)


## RTL LOGIC UP COUNTER
![image](https://github.com/user-attachments/assets/7e4ed521-cd29-4bc3-b42a-2ef7978dd475)

## TIMING DIAGRAM FOR IP COUNTER
![image](https://github.com/user-attachments/assets/8bd76903-5497-443c-84f9-b2148259439f)

## TRUTH TABLE
![image](https://github.com/user-attachments/assets/02a77de2-a807-4226-ab57-b3eef9f88c8a)

## RESULTS
the given program for flipflops and verify its truthtable in quartus using verilog programming.
