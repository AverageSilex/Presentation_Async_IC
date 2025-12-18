# Part I - Introduction to integrated circuits

## Abstractions
* System
* Data/Control flow (pipeline)
* Behavioral / Structural modules
* Netlist / Gate level
* Physical design, masks and Waffer

## Design Families

* Flexibility vs Performance

### CPU
* SISD
* Instruction Set Architecture (System) and programs
* Van Neumann / Harvard architecture (System)
* 5 stage execution pipeline

### GPU
* SIMD
* Parallelism vs serial

### Coprocessor / Hardware Accelerator
* System BUS
* IPs

### FPGA
* Reconfigurable hardware
* LUT architecture (Structural / Gate level)

### ASIC
* System on Chip with IPs
* Multi-abstraction level design

## Design Flow

* Successive refinement

### Verification and Validation
* Formal verification
* Functional verification
* FPGA prototypes

### Synthesis
* High Level Synthesis
* Logical Synthesis (Zoom)
- Boolean Algebra
- Logic gates
- Transistor level
- Mask

### Physical
* Place and Route
* PVT ?

## (Optional) Monopoly / Oligopoly

* Problem foundries
* Problem PDK
* Problem EDA
* OPENROAD and CHIPS

# Part II - Asynchronous circuits

## Linear pipeline or digital Fordism
* Stages that operate in parallel akin to an assembly line
### Concepts
* Latency
* Throughput
* Parallelism
* Concurrency

## Clock-driven
* Data propagation through global synchronization
* Timing assumption in synchronous circuits
- Critical Path
- Worst case timing assumption
- Setup
- Hold
* Problem with synchronous designs : large clock tree <-> clock skew; Clock Domain Crossing (GALS); Process Voltage Temperature

## Event-driven
* Local synchronization
- Handshakes
* Control flow (modelization through communicating channels)
- Control primitives

## Transactions at the gate level
* DI and QDI
* Mueller gate / C-element
* PRS and STG ?

## Transaction at the pipeline level
* Bundled-Data with matched delay : Setup and Hold
* Timing constraints in Bundled-Data
- Relative Timing Constraints (RTC)
- Local Clock Sets (LCS)