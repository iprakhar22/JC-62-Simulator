# JC-62-Simulator
A simulator of the JC-62 microcomputer

This is a project made by me along with some help my from my group members as a final project of Computer Organisation and Architecture. The frontend of the simulator was made using the tkinter python framework and the basic backend and all the functionalities are implemented using basic logic in python.
The project is currently incapable of handling any exception/bug.

The machine code should be written in capitals and error free. Use single spaces between instructions.
The memory mapping is done by double clicking a tuple in the memory section, editing the values, and then pressing "Set Values". 

**Example:**

After pressing 2C memory block;

2C  X  123

**To use:**
~~~~
python JC-62\ Simulator.py
~~~~

**Instructions supported by the JC-62 machine :**

* LDA X - Load into the accumulator the value mapped at label X
* STA X - Store the value of accumulator at the memory location at label X
* MBA - Copy the value of accumulator to register B
* ADD - Add the values of accumulator to register B and write-back into accumulator
* SUB - Subtract the values of accumulator from register B and write-back into accumulator. Negative Flag (NF) is set high(1) in case the value obtained is negative.
* JMP AH - Jump to address A in hexadecimal base.
* JN AH - Jump to address A in hexadecimal base if negative flag (NF) is set high.
* HLT - Halt the program.


Sample Code to Test: (performs addition of X and Y and stored back at location Y. Map values into X and Y before running) 
~~~~
LDA X
MBA
LDA Y
ADD
STA Y
HLT
~~~~


Requesting exception-handlers for the program and removal of bugs.
