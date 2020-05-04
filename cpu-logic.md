Computer Architecture and Logic notes go here

### Video Notes
 Computers have 4 main components
 1. Input
    + types of input: keyboard, voice, camera, 
 1. Storage
    + all inputs are stored in **binary**, because they can all be measured in numbers
 1. Processing
    + series of commands takes place
 1. Output
    + dependent on steps before it 

> New types of inputs and outputs let computers interact with the world in entirely new ways. 

### The math behind binary
In "regular" arithmetic we work in mod 10 while computers do everything mod 2. 

In base 10 place values we have the ones place, tens place, hundreds place, etc which is the same as 10^(0), 10^(1), 10^(2), 10^(3), etc. 

In base 2 place values go by powers of 2 aka 2^(0), 2^(1), 2^(2), 2^(3), etc. So a conversion method would be:

> Suppose x is an integer, divide x by 2 keeping track of the quotient and remainder. Continue dividing the quotient by 2 until you can't any longer, still keeping track of the remainders. With the list of remainders, write them in reverse order to receive the binary equivalent. 

Ex: Convert 12 from base 10 to base 2
Division|Quotient|Remainder
--------|---------|--------
12:2|**6**|0
**6**:2|**3**|0
**3**:2|**1**|1
**1**:2|0|1

Thus 1100 is equivalent to 12 in base 2. 


**Wires** in these cases represent places as in place values or digits. The more wires allowed, the more information that can be used and stored. 

## Circuits
They modify and process information taken from 1' and 0's. Complicated circuits take multiple signals and combine them for different results. 

A **not** circuit is one where the output is NOT the same as the input. 

## Hardware + Software

**Central Processing Unit** is the master chip that controls all the other parts of the computer. Inside of a CPU it has circuits that do simple math and logic, send and receive information, and knows how/when to use each one. 

*Software* tells the CPU what to do. The operating system is the master porgram that manages how software uses the hardware of the computer. The **OS** is switching through each application, program, command and is all commanded by the programmer. 




