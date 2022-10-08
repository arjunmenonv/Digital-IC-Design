# Digital-IC-Design
Schematic and Layout libraries of digital logic gates and cells. Assignments and Project from EE5311 Digital IC Design course at IIT Madras. 
Aug-Nov 2021

Collaborators: [Arjun Menon V](https://github.com/arjunmenonv), [Srinivas R](https://github.com/srinivasrdhkrshnn) and [Ashwanth S]()


To run simulations for the schematic and layout files included in the library, replace the include path with path to the model file in the .include command.

## Tools used:
- [Electric VLSI](https://www.staticfreesoft.com/productsFree.html): for schematic and layout generation
- [Java 3D](https://www.oracle.com/java/technologies/java-archive-downloads-java-client-downloads.html#java3d-1.5.1-oth-JPR): for layout visualisation in 3D
- [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html): SPICE simulation 

## Repo Contents:
- [Assignment 1](https://github.com/arjunmenonv/Digital-IC-Design/tree/main/Assignment%201): Inverter, NAND2 aand AND2 logic gates. 
- [Assignment 2](https://github.com/arjunmenonv/Digital-IC-Design/tree/main/Assignment%202): Carryout circuit of an Adder.
- [Assignment 3](https://github.com/arjunmenonv/Digital-IC-Design/tree/main/Assignment3): Schematic and Layout of a Full Adder circuit.
- [Assignment 4](https://github.com/arjunmenonv/Digital-IC-Design/tree/main/Assignment4): Schematic Design of an 8-bit signed Carry Save multiplier using a Ripple-Carry adder in the Vector Merge stage. Optimal sizes of constituent cells (NAND, Sum-Generation and Carry-Out) were found by modelling the critical path of the circuit and evaluating the worst case delay for all possible size combinations.
- [Project](https://github.com/arjunmenonv/Digital-IC-Design/tree/main/Project): Layout Design and Simulations of the 8-bit signed Carry-Save Multiplier. Also includes a single-stage pipelined version of the schematic, that enables a 1.79x speedup of the clock (resulting in throughput improvement). Flip-Flops based on the dynamic C2MOS flop topology was used for the pipeline stage. Additionally, alternate vector merge stages of the Carry-Skip adder were designed using the Carry-Skip adder and Carry-Lookahead adder architectures. Layout GDS is saved as 11.gds
  - project.jelib: Schematic and Layout designs of the non-pipelined Multiplier and its constituent cells. The layout occupies an area of 2248 units x 409 units, where 1 unit = 11nm (for the 22nm process). This corresponds to a layout aspect ratio of 5.5:1. The layout is exported into GDS format a
  - CarrySkipMult.jelib: Schematic design of Carry Skip Adder and Design-Under-Test schematic incorporating the adder into the multiplier. 
  - CSM_pipeline.jelib: Schematic design of C2MOS Flip Flop and DUT schematic of a single stage pipelined CSM.
