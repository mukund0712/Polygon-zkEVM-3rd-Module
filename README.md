# Custom Multiplier Circuit using CIRCOM
## Introduction
This CIRCOM code defines a customizable multiplier circuit template called Multiplier2. This circuit assesses whether the output signal 'q' is the outcome of multiplying input signals 'a' and 'b'. The Multiplier2 circuit employs custom logic gates for AND, NOT, and OR operations, allowing for versatile logic design.

## Prerequisites
To effectively comprehend and execute the custom logic circuit, a basic understanding of digital logic and logic gates (such as AND, NOT, OR) is necessary. Furthermore, familiarity with a hardware description language (HDL) simulator that supports Verilog or VHDL is recommended.

## Circuit Description
### Input Signals
The Multiplier2 circuit template involves the following input signals:

**a:** Represents the first operand input signal.

**b:** Represents the second operand input signal.

## Intermediate Signals
Within the circuit, two intermediate signals are generated:

**x:** This signal denotes the outcome of the logical AND operation between signals 'a' and 'b'.

**y:** This signal represents the result of the logical NOT operation performed on signal 'b'.

**Output Signal**
The ultimate output signal is labeled as:

**q:** This signal reflects the result of the logical OR operation conducted between signals 'x' and 'y'. It essentially determines whether the signal 'q' corresponds to the product of 'a' and 'b'.

## Custom Logic Gates
The circuit employs the subsequent custom logic gates:

**AND():** Executes the logical AND operation between two given input signals 'a' and 'b'.

**NOT():** Carries out the logical NOT operation on the provided input signal 'in'.

**OR():** Executes the logical OR operation between two specified input signals 'a' and 'b'.

## Circuit Logic
The operational logic of the Multiplier2 circuit can be outlined as follows:

1. The input signals a and b are interlinked with the input of the AND gate (andGate).
2. The outcome of the AND gate, designated as x, is interconnected with one of the inputs of the OR gate (orGate).
3. The input signal b is linked with the input of the NOT gate (notGate).
4. The output of the NOT gate, denoted as y, is connected to the other input of the OR gate (orGate).
5. The final output of the OR gate, labeled as q, provides information about whether 'q' signifies the multiplication of 'a' and 'b'.
   
## Usage Instructions
To incorporate the Multiplier2 circuit into your HDL simulator, adhere to these steps:

1. Download the relevant source code files from the provided repository.
2. Set up your HDL simulator and establish a new project.
3. Integrate the acquired source code files into your project.
4. Instantiate the Multiplier2 module within your designated testbench or primary file.
5. Supply inputs 'a' and 'b' to the Multiplier2 module.
6. Extract the output 'q' from the Multiplier2 module to ascertain the multiplication outcome.
## Authorship and License
**Author:** Mukund Singh Parmar

**License:** This circuit is governed by the MIT License. For license details, refer to SPDX-License-Identifier: MIT.
