# Learning
All codes/ projects worked on for learning tasks are to be done in this directory, create a separate folder for each learning task and organize its components accordingly.

## Directory Structure

- [Embedded C](Embedded%20C) 
- [Hardware Description Language](HDL)
  - [Verilog](HDL/Verilog)
  - [VHDL](HDL/VHDL)
- [High-Level Synthese](HLS)
- [Printed Circuit Board](PCB)

## General Terminology
<!--Primary contributor Durgaprasad-->
1. SRAM (Static RAM): A RAM using flip-flops to store data. It 
    is volatile, faster and more expensive than traditional DRAM’s and usually
    used for cache data. Consume low power when idle, high power when reading
    or writing data.Do not require data refresh mechanism.

2. DRAM (Dynamic RAM): Uses a combination of a capacitor
   and a transistor as a memory cell. It is a volatile memory and requires an 
   external refresh circuit to restore the amount of charge on the capacitors 
   periodically. It is much denser on the chip than SRAM due to its simple memory
   cell. Typically used as primary memory modules. Consume high power due to
   the need to be refreshed frequently.

3. BGA (Ball Grid Array): A type of surface mount packaging which uses an array of small balls of soldier covering the entire/a part of  the IC’s bottom to connect it to the PCB. The IC’s after placing on the pads are heated using an oven or IR heater to solder the IC to the PCB. The advantages over dual in-line or flat packaging include lower lead resistance and hence lower heat dissipation, lower lead inductance, denser pin configuration, efficient flow of heat over the PCB due to the contacts being spread over a larger area. Disadvantages include lack of flexibility(required to deal with thermal expansion and mechanical stress), difficulty in finding faulty connections and no room for changes once soldered.

4. Redundancy: Use of multiple hardware or software systems with the same functionality so as to make the system more reliable with back-ups available in case of failure. Usually implemented for vital components of any system. Generally triplication is used so that wrong response from one component can be overruled by the two other components. This may add up to the complexity of the system and hence lead to more maintenance costs and decreased efficiency. Data(information) redundancies are used for error detection and correction. 
Dissimilar redundancy: Uses two different methods for the same task as there is very low chance for two different implementations to have same problems and fail at the same time. 

5. DMA (Direct Memory Access): A method of data transfer in which peripheral devices can read and write information directly from the memory without the data being processed by the processor. This increases the speed of the memory operations. The process is controlled by a DMAC(DMA controller).
 
6. HLS (High Level Synthesis): It is a process in which an algorithm written in a high level programming language (usually C++) is interpreted and a digital hardware is created which implements the same algorithm. The C++ code is analyzed and transcompiled into a register transfer level design in a Hardware description language(HDL)  which is then implemented by logic gates using a logic synthesis tool.
   
7. Volatile Memory: A type of memory device in which the stored data is lost when the power supply is stopped and is hence used for storing data temporarily. It is much faster and power efficient in terms of reading and writing data to volatile memory as compared to that of non- volatile memory. It has less storage capacity and costlier as compared to its non-volatile counterpart. Eg: RAM, Cache data.

 Non-Volatile memory: A type of memory device in which the data remains 
 intact even after power to the device is switched off and hence used for
 permanent/long term storage. 

8. BRAM (Block RAM): A block RAM is a discrete part of the FPGA and is used to store large amount of data on FPGA’s  

9. LUT (Look Up Table): A lookup table is the customized truth table of a FPGA logic block which determines the behaviour/combinatorial logic of the logic block. The input lines are the address line which point to the desired output on the RAM on which the LUT is loaded. This saves the need of complete implementation of the logic using gates.

10. COTS (Commercial Off-The-Shelf): Refers to hardware or software   
products that are readymade and available in the market and which can be
used for a wide range of applications by different organizations without
much customization. 
          
11. CMOS (Complementary Metal Oxide Semiconductor): It is technology used 
to produce integrated circuits. The term MOS stands for transistors(MOSFET) and complementary stands for two types of (P-type and N-type) semiconductor used. These are known for their energy efficiency and minimal heat production.

12. Testbench: It is used to simulate a block of code( in HDL) using clocks, inputs, resets etc, allowing you to  look at each signal in the FPGA. This allows us to ensure proper working of the synthesised hardware and also debug it.

13. Databuffer: A region of memory used to store data temporarily before  transferring between devices or processes or before processing it. Usually used when there is a difference between the rate at which data is received and it is sent or processed. Typically RAM used for the purpose  

14. Bitstream: A sequence of bits.

15. CCD (Charge Coupled Devices): A technology used in IC’s which contains an array of connected capacitors which can transfer charge under the control of an external circuit. Generally used for image sensors in digital imaging. 

