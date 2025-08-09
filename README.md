# SPI-slave-with-single-port-RAM
SoC SPI Slave with Single-Port RAM
Overview
This project implements a Serial Peripheral Interface (SPI) slave integrated with a Single-Port RAM in Verilog HDL as part of a System-on-Chip (SoC) design. The SPI slave acts as a communication interface between an SPI master and the internal RAM, allowing the master to perform read and write operations to the memory. The design supports full-duplex communication in SPI Mode 0 (CPOL = 0, CPHA = 0), with parameterized RAM depth and data width.

Features
SPI Slave Interface

Supports SPI Mode 0 (CPOL = 0, CPHA = 0).

Handles MOSI (Master Out Slave In), MISO (Master In Slave Out), SCLK (Serial Clock), and CS_n (Chip Select).

Full-duplex data transfer.

Synchronization to SPI clock domain.

Single-Port RAM

Parameterized depth and data width for flexibility.

Supports both read and write operations via SPI commands.

Synchronous memory operations.

Command Protocol

Write Command: Allows the SPI master to write data into specific memory addresses.

Read Command: Allows the SPI master to read stored data from specific memory addresses.

Error Handling

Invalid command detection.

Out-of-range address handling.
