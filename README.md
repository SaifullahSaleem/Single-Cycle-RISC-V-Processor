# Single-Cycle-RISC-V-Processor
This project is a Verilog implementation of a **Single-Cycle RISC-V Processor** as part of the **COAL (Computer Organization & Architecture Lab) course**. It supports fundamental RISC-V instructions including arithmetic, memory operations, and branching.  

## Features  
- **Single-Cycle Execution**: Completes one instruction per clock cycle.  
- **RISC-V ISA Compatibility**: Implements a subset of the RISC-V instruction set, including:  
  - R-type (add, sub, and, or)  
  - I-type (load)  
  - S-type (store)  
  - B-type (branch)  
- **Key Components**:  
  - **Program Counter (PC)**  
  - **Instruction Memory**  
  - **Register File**  
  - **ALU (Arithmetic Logic Unit)**  
  - **Control Unit**  
  - **Immediate Generator**  
  - **Data Memory**  
  - **Multiplexers and Adders**  

## File Structure  
- `final_code.v` - Verilog source code for the processor, including all modules.  

## Modules Overview  
- **Program Counter (PC)**: Holds the address of the current instruction.  
- **Instruction Memory**: Stores instructions in machine code format.  
- **Control Unit**: Generates control signals based on the opcode.  
- **Register File**: Stores register values and supports read/write operations.  
- **ALU**: Performs arithmetic and logical operations.  
- **Immediate Generator**: Extracts and sign-extends immediate values.  
- **Data Memory**: Handles load and store instructions.  
- **Multiplexers**: Control data flow based on control signals.  

## Instructions Supported  
| Type  | Instructions |
|-------|-------------|
| R-type | `add`, `sub`, `and`, `or` |
| I-type | `lw` (Load Word) |
| S-type | `sw` (Store Word) |
| B-type | `beq` (Branch if Equal) |

## How to Run  
1. **Simulate in ModelSim, Xilinx Vivado, or Quartus Prime**  
   - Load the Verilog files.  
   - Compile and run the simulation.  
   - Observe the register/memory updates after each cycle.  
2. **Modify Instruction Memory**  
   - Change predefined instructions in the `INST_MEM` module for different test cases.  


