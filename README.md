

# 3D-Bezier-patch-ARM-NEON-Assembly
A 3D Bezier creator in full ARM NEON Assembly


Background

In 1987 I started programming Assembly language on the first Desktop computer with an ARM Processor and its first OS,
The ARM2 with the Arthur OS, later to be called RISCOS

My motivation to start learning Assembly language was initiated by a frustration to be stuck with a very slow triangle fill command in BASIC. It took me weeks to understand and finish the assembly algorithm, but the result eventually was 70 times faster. I fell in love with the architecture of the chip and the extremely clever setup.
In 1991 I quit programming as a hobby as I was starting my carreer in the army and later at airports. Only a few years ago, when the RaspBerry Pi was launched, together with the original RISCOS, I bought one and was immediately ready to go.
I set my challenge to learn the NEON instruction set and to create the fastest possible 3D-Bezier-patch modeller. Always been interested in curved surfaces....

The program underneath was written on the Cortex A7 ARM cpu in RISCOS 5.23

*********************************************************************************************************************
RISCOS:

RISCOS is -unfortunately- hardly used anymore. For me it was the only way to start programming immediately without having to deal with and learn other OS's with there IDE's to get to the same result. 
Being aware of writing software in a very rare OS, I created a specific setup of the program that makes it relatively easy to port it to any kind of ARM v7 (or later) device, through modern IDE's.
RISCOS has implemented a lot of system calls to make it easy for the programmer, even in assembly language. In my program I eliminated almost every system call. There are only two left:
1. RISCOS has a very rudimentary way of dealing with the screen. In my program I had to use a system call to retrieve the hard address of the screenbuffer and its size.
2. In order to use the floating point units in the Cortex A7, I had to create a VFP-context that I was only able to do throug a system call.
All the rest is clean assembly with mnemonics that are indentical in other and newer assemblers.





**********************************************************************************************************************
The core code set up and discription


more to follow
