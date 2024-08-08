# Physical Design from Netlist to GDSII in ICC/ICC2

Welcome to the repository for the "Physical Design from Netlist to GDSII in ICC/ICC2" course. This repository contains the completed lab exercises, which cover various stages of the physical design flow, including SPICE simulation, synthesis, floorplanning, placement, clock tree synthesis, signal routing, static timing analysis, and design optimization using OpenRoad.

## Lab Descriptions

### Lab 1: SPICE Simulation

This lab focuses on SPICE simulation of an inverter cell to analyze its behavior under different conditions.

#### Exercises:
1. **Simulation of an Inverter Cell (4x, 7nm)**
   - Run SPICE simulations to measure delay and transition time.
   - Plot input slew vs. rise/fall delay and input slew vs. rise/fall transition time.

2. **Simulation with Different Load Capacities**
   - Simulate the inverter with various load capacitors (5ff, 10ff, 20ff, 25ff).
   - Plot output load vs. rise/fall delay and output load vs. rise/fall transition time.

### Lab 2: Synthesis of RISC-V Core

This lab covers the synthesis of the RISC-V core using two different technology libraries: 28nm and 7nm.

#### Exercises:
1. **28nm Library Synthesis**
   - Perform synthesis using the 28nm library and analyze cell area, timing slack, and number of cells.
   
2. **7nm Library Synthesis**
   - Perform synthesis using the 7nm library and compare the results with the 28nm synthesis in terms of cell area, timing slack, and number of cells.

### Lab 3: Floorplanning & Placement Basics of RISCV ORCA

This lab introduces floorplanning and placement of the RISCV ORCA design.

#### Exercises:
1. **Initialize Floorplan**
   - Set up the floorplan, place macros, and connect power and ground nets.

2. **Placing Macros**
   - Optimize macro placement and report congestion, routing, and timing.

### Lab 4: Floorplanning & Placement Optimization

This lab focuses on optimizing the floorplan and placement for better performance and reduced congestion.

#### Exercises:
1. **Run Floorplan & Placement**
   - Execute floorplan and placement scripts and analyze the results.

2. **Run Floorplan & Placement (Large Area)**
   - Compare the results of different placement strategies and optimize the design.

### Lab 5: Clock Tree Synthesis (CTS)

This lab involves running clock tree synthesis on the ORCA design to balance clock distribution.

#### Exercises:
1. **Run CTS on ORCA Design**
   - Execute the CTS script and analyze the clock tree quality and timing.

### Lab 6: Signal Routing

This lab covers signal routing to complete the physical design of the ORCA core.

#### Exercises:
1. **Run Signal Route on ORCA Design**
   - Execute the signal routing script and analyze the routing quality and timing.

### Lab 7: Static Timing Analysis (STA)

This lab focuses on performing static timing analysis before and after layout.

#### Exercises:
1. **Prelayout STA**
   - Execute prelayout STA script and analyze timing.

2. **Postlayout STA**
   - Execute postlayout STA script and analyze timing.

### Lab 8: Design Optimization Using OpenRoad

This lab involves optimizing the RISC-V design using the OpenRoad tool suite.

#### Exercises:
1. **Run RTL to GDS Flow**
   - Execute the OpenRoad flow and optimize the design for power, performance, or area.

## Directory Structure

The repository is organized as follows:
lab1 /spice_simulation - invx4_tt0p65v-40c.spi - invx4_tt0p65v-40c_out.mt0 - invx4_tt0p65v-40c_out.tr0

/lab2 /synthesis - dc_28nm.tcl - dc_28nm.log - dc_7nm.tcl - dc_7nm.log

/lab3 /physical_design - setup.tcl - tluplus_optimization_ctrl.tcl - pad_cell_cons.tcl - insert_pad_filler.tcl - connect_pg.tcl - preplace_macros.tcl - fp_placement.tcl - fp_placement_large_area.tcl

/lab4 /physical_design - fp_placement.tcl - fp_placement_large_area.tcl

/lab5 /physical_design - run_cts.tcl

/lab6 /physical_design - run.tcl

/lab7 - prelayout_sta.tcl - postlayout_sta.tcl

/lab8 /openRoad_flow - config.mk - Makefile - results/ - reports/ - logs/









