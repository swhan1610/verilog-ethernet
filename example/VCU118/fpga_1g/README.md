# Verilog Ethernet VCU118 Example Design

## Introduction

This example design targets the Xilinx VCU118 FPGA board.

The design by default listens to UDP port 1234 at IP address 192.168.1.128 and
will echo back any packets received.  The design will also respond correctly
to ARP requests.  

FPGA: xcvu9p-flga2104-2L-e
PHY: TI DP83867ISRGZ

## How to build

Run make to build.  Ensure that the Xilinx Vivado toolchain components are
in PATH.  

## How to test

Run make program to program the VCU108 board with Vivado.  Then run
netcat -u 192.168.1.128 1234 to open a UDP connection to port 1234.  Any text
entered into netcat will be echoed back after pressing enter.  


