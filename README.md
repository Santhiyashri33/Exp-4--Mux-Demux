# Exp-4-Mux-Demux
# Design and Verification of 2:1 Multiplexer and 1:2 Demultiplexer
## Aim
To design and verify a 2:1 Multiplexer and a 1:2 Demultiplexer using Verilog HDL.
## Theory / Synopsis
A 2:1 Multiplexer (MUX) selects one of two data inputs, A or B, and routes it to a single output Y based on the value of the select line S. A 1:2 Demultiplexer (DEMUX) performs the reverse operation: it routes a single data input D to one of two outputs, Y0 or Y1, based on the select line S.
Boolean Functions
### 2:1 Multiplexer:
•	Y = S'.A + S.B
### 1:2 Demultiplexer:
•	Y0 = S'.D
•	Y1 = S.D
## Files to be Created

<img width="575" height="65" alt="image" src="https://github.com/user-attachments/assets/04c2d90c-0b6b-4b35-b603-d0e10e1e4f00" />

## Design / RTL Program


## **Testbench Program



## Truth Table

### 2:1 Multiplexer

<img width="573" height="154" alt="image" src="https://github.com/user-attachments/assets/96dd3fa2-7747-402d-b88f-17c11e28fcbb" />

### 1:2 Demultiplexer

<img width="583" height="90" alt="image" src="https://github.com/user-attachments/assets/4bc21b52-1db5-4302-afab-ebb0b9d5a74b" />

## Simulation Procedure

STEP 1 – Open Terminal
Open a terminal in the experiment folder.

STEP 2 – Load Synopsys Environment
source /synopsys/start.sh

STEP 3 – Compile Using VCS
vcs mux_demux.v mux_demux_tb.v -full64
If compilation is successful, VCS generates the simulation executable:
simv

STEP 4 – Run Simulation
./simv
The terminal displays the input combinations and corresponding outputs Y, Y0, and Y1.
A VCD waveform file is also generated:
mux_demux.vcd

STEP 5 – Open DVE

dve -full64
Other option
dve -full64 &
A DVE environment will open.
DVE Waveform Verification
<img width="1920" height="1080" alt="Screenshot (102)" src="https://github.com/user-attachments/assets/4cf0306d-6ce7-4e29-bed4-53552e0e19a4" />
<img width="1920" height="1080" alt="Screenshot (103)" src="https://github.com/user-attachments/assets/93f55749-1a22-43b4-8658-c73921c16c18" />


## Expected Result
<img width="909" height="378" alt="Screenshot (101)" src="https://github.com/user-attachments/assets/edfbd063-e585-4e13-bef5-38f5a75b8c95" />



## Result

Thus, the 2:1 Multiplexer and 1:2 Demultiplexer were designed, implemented using Verilog HDL, successfully simulated using Synopsys VCS, and verified using Synopsys DVE.



