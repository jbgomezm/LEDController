# Observations

- Configuring the environment takes time. Even with almost self-contained alternatives such as OSS-CAD_suite, getting everything to work properly can take up to a couple hours. 
- Tool assertion is important. It is not sufficient to check that things are installed; they should be working. Tools to test for simulation: Yosys, iverilog, verilator*, gtkwave/surfer. Tools for deployment: NextPNR with himbaechel extensions for Gowin/ Apicula.
- Makefile tool familiarity cannot be taken for granted. Most likely than not, people in "training the trainer" are not going to be familiar with make and its syntaxis.
    + Same can be said if TCL scripts are involved.
- Verilog is a must. If not taken as such, the scope of the course shall be extended to cover HDL basics.
- VS Code integration is optional, but probably desired. It also eases the AI integration for code generation and review.
- A possible way to approach the introductory task is to:
    + Configure the environment.
    + Test the subsystem (Yosys, NextPNR, Apicula). It can be performed using a simple design.
    + Configure VS Code integration. Test with an AI generated design and TB.
    + Introduce a graphical depiction of the RISC V core, particularly the one to be used (Quark?). 
    + Show the relationship of the core with a SoC implementation.
    + Introduce the project tree of the SoC implementation.
    + Work with a template for Makefile and SoC. Optionally, include a template for SoC_tb as well.
    + Run the SoC simulation (preset).
    + At this point, the task of designing a new peripheral for the SoC can begin.
    