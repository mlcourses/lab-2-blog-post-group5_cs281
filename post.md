# Lab 01: Journey into Hardware - Digital Design Odyssey

## Overview and Motivation

Welcome to our second lab! In this lab, we delve into the foundations of digital design, focusing on multiplexers and adder circuits. Starting with a 2-to-1 multiplexer constructed from basic logic gates, progressing to a 4-to-1 multiplexer using the 74150 chip, and integrating Arduino for practical testing, we aim to unravel the core principles of digital circuits in an accessible manner. The motivation is to demystify these components, fostering a deep understanding of the binary foundations that power digital technologies. By the end, you'll have hands-on experience with multiplexers, insight into their applications, and a fundamental grasp of how to design and test digital circuits.

## What We Did In The Last Lab

In the previous lab, we familiarized ourselves with the PB-503 breadboard prototyping stations and Arduino microcontroller systems. The activities involved exploring the breadboard's features and integrating the Arduino for embedded processor control. By the end of the lab, you should have mastered working with components like the PB-503 breadboard and its features, LEDs, resistors, integrated circuit chips, requiring reference to IC data sheets, as well as programming the Arduino board and use it to automate the testing process with the breadboard. For more in-depth lab details, refer to the previous lab in this [URL](https://github.com/mlcourses/lab-1-blog-post-group5_cs281/blob/main/post.md)

## Lab Objectives

1. Master Prototyping with PB-503 Breadboard.

1. 2-to-1 Multiplexer construction.

2. Implement a 4-to-1 Multiplexer with the 74150 chip.

3. Arduino Testing for 4-to-1 Multiplexer.

4. Desgin and Build a 1-bit Adder Circuit.

## Materials

- PB-503 breadboard prototyping station

<img src="./assets/PB-503.png" alt="breadboard" height="450" width="600"/>

- Arduino microcontroller kit

<img src="./assets/Arduino_kit.png" alt="arduino_kit" height="450" width="600"/>

- 7404 NOT gate IC

- 7408 AND gate IC

- 7432 OR gate IC

- 7486 XOR gate IC

- 74150 MUX chip

<img src="./assets/logic_gates.png" alt="logic gates" height="450" width="500" />

- IC data sheets

- Wires and connection tools

<img src="./assets/wiring_kit.png" alt="arduino_kit" height="450" width="500"/>

- Logic Probe
- Arduino IDE software
- Laptop or device for programming and connecting to the Arduino

## Project Steps

### UNDERSTANDING A MULTIPLEXER

- A multiplexer, often called a "MUX", is a sophisticated selector crucial for managing signals in digital systems. Imagine it as a control panel with various input buttons (data inputs), and the multiplexer acts as the conductor, choosing which specific signal gets transmitted to the output.

- Here's the key: input lines carry actual data signals, while the selector lines control which input takes the spotlight. This distinction between control and data is fundamental when it comes to Integrated Circuits (ICs).

- Multiplexers vary in size, accommodating different numbers of inputs in powers of 2. The number of selector lines is log2(n), where n is the number of data inputs. So, for example, a mux with 2 inputs will have 1 select line and one with 4 inputs will have 2 select lines.

- We name the mux by the number of data lines. So we can have common sizes such as 2-to-1, 4-to-1, 8-to-1, 16-to-1 muxes.

### BUILDING A 2 TO 1 MUX

- Here is an outline of what a 2 to 1 mux might look like: 

<img src="./assets/2-to-1_outline.png" alt="arduino_kit" height="350" width="600"/>

- In this first section of the lab, we are to build a 2 to 1 multiplexer using the 7408 AND, 7432 OR, and 7404 NOT gate. 

- Before we delve into the wiring portion, we can draw a logical outline for the mux based on its Boolean expression:

<img src="./assets/2-to-1_logic.png" alt="logic diagram of 2 to 1 mux"  />

- When S (select line) is low (off), it selects line A for the output Y . When S is high, then the output Y copies input B

<img src="./assets/2-to-1_mux_1.png" alt="logic diagram of 2 to 1 mux"  />

- Above is the wiring design of our 2 to 1 mux. with the 7408 AND gate IC top left, the 7404 OR gate IC on the bottom and the 7432 OR gate IC on the right. 

- Notice that instead of using 2 separate 7408 AND gate IC, we decided to use just 1 IC and opt for 2 independent small AND gates in the IC, each with 2 inputs and 1 output to reduce the wiring complexity of our digital design. 

- Relating to the logic outline of the mux, we use our PB-503 breadboard's S5 and S6 logical switches as our 2 data input lines, representing A and B while the 7404 NOT gate IC takes switch S1 as our select line. 

### BUILDING A 4 TO 1 MUX



## Testing

## Conclusion

In wrapping up this lab, we've delved into the intricate world of multiplexers, adder circuits, and digital design. From constructing a 2-to-1 mux with basic gates to utilizing a 74150 chip for a 4-to-1 mux, we've expanded our understanding of these fundamental components. Integrating Arduino into the mix not only showcased practical applications but also emphasized the dynamic nature of digital systems. As we delved into the design and implementation of a 1-bit adder circuit, the lab offered a holistic experience in digital circuitry. The challenges and successes encountered in building, testing, and troubleshooting these circuits provided invaluable insights into the nuances of hardware design. Overall, this lab has laid a solid foundation for comprehending multiplexers, adders, and the broader landscape of digital design in computer systems.




