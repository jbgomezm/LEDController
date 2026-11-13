# LED Controller for a RISC V Soft Core

--- 

## Project Goals

### Main Goal

Design, implement and test a peripheral compatible with the femtoRV bus design used in the femtoUN approach, such that enables us to drive a FM6124DJ based LED matrix controller with 64x32 RGB LEDs.

### Specific Goals



---

## Tasks

- Implement a dummy peripheral that stores a few register values addressed to it via the bus of the FemtoRV.
    + Write the dummy peripheral.
    + Implement a test bench for the dummy peripheral, testing proper address decoding, data storage and retrieval.
- Implement a first version of the LED controller interface, able to generate the control signals for the driver.
    + Implement a test bench for the first version of the LED controller.
- Create a SoC with a UART interface and the LED controller.
- Test the SoC with an echo program, in order to assert that both the processor and the bus are working properly.
    + Create a basic c program that performs the echo.
    + Compile and create the corresponding hex file.
    + Test the program using a verilog testbench.
    + Burn and run the SoC with the echo program in the FPGA.
- Test the SoC with a basic LED sequence (blanking, colorbars).
    + Create a basic c program that generates the blanking sequence and the colorbar sequence.
    + Compile and create the corresponding hex file.
    + Test the program using a verilog testbench.
    + Burn and run the SoC with the test program.

---

## Uncertainties

- How is the LED matrix powered? (input voltage and current)
- What is the controller protocol?
- 