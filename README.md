# ECE 128 Lab 1: 8-to-1 Multiplexer
This project implements an 8-to-1 multiplexer (MUX) using Verilog HDL. The MUX has eight data inputs, three select inputs, and one output. The three select inputs determine which of the eight data inputs is passed to the output

The 8:1 MUX was implemented using three different Verilog modeling methods:
- Structural modeling
- Behavioral modeling
- Dataflow modeling

A testbench was used to simulate and verify the functionality of the MUX. The design was also implemented and tested on a Basys 3 FPGA board

## Simulation
The design was simulated using Xilinx Vivado. To run the simulation:
1. Create or open the project in Vivado
2. Add the desired MUX Verilog file as a design source
3. Add the testbench as a simulation source
4. Run Behavioral Simulation
5. Use the simulation waveform to verify that the output matches the input selected by the three select signals

The testbench tests all eight possible combinations of the select inputs

## FPGA Implementation
The design was implemented on a Basys 3 FPGA board using Vivado

To implement the design:
1. Add the Verilog source file and Basys 3 constraints file to the Vivado project
2. Assign the data inputs and select inputs to switches on the Basys 3
3. Assign the MUX output to an LED
4. Run synthesis and implementation
5. Generate the bitstream
6. Connect the Basys 3 and open Hardware Manager
7. Program the FPGA with the generated bitstream
8. Test different input and select combinations using the switches and verify the output using the LED
