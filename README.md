FPGA-Based Hamming Code Error Detection and Correction System

Introduction

When data travels from one device to another, errors can happen because of:

Noise

Signal disturbance

Weak connections

Hardware problems


Even one wrong bit can change the entire data.

This project explains how Hamming Code helps in:

Finding errors

Correcting errors

Making communication more reliable


The system is studied using FPGA concepts and digital logic.


 Objectives

Learn what Hamming Code is

Understand how errors happen in data transmission

Learn the use of parity bits

Detect single-bit errors

Correct single-bit errors

Study FPGA-based error correction systems


Problem Statement

In communication systems:

Data may get corrupted during transmission

Simple parity checking can only detect errors

Some error correction methods are too complex


So, we need a system that:

Detects errors

Corrects errors

Works fast

Uses less hardware


What is Hamming Code?

Hamming Code is an error detection and correction technique developed by Richard Hamming.

It works by adding extra bits called parity bits to the original data.

These parity bits help to:

Identify the error position

Correct the wrong bit automatically


Example

4 data bits + 3 parity bits = 7-bit code


This is called (7,4) Hamming Code.


Working of the System

1. Encoder

The encoder:

Takes original data

Adds parity bits

Creates protected data


2. Transmission

The data is sent through a communication channel.

Sometimes errors occur during transmission.

3. Decoder

The decoder:

Checks parity bits

Finds the error

Corrects the error

Gives correct output data



 Main Blocks Used

Hamming Encoder

Error Generator

Syndrome Checker

Error Corrector

Decoder


 Literature Review

Paper 1

Used basic Hamming Code.

Simple design

Low hardware usage

Slower processing


Paper 2

Focused on FPGA implementation.

Better reliability

Uses parity generation


Paper 3

Implemented hardware using CPLD.

Fast operation

Useful in modern devices


 Research Gap

Existing systems mainly correct:

Only single-bit errors


Problems:

Cannot correct multiple errors together

Power usage is not discussed

Security against intentional errors is limited


Tools Used

Verilog HDL

Xilinx Vivado

FPGA Design


Project Includes

Block diagram

Encoder and decoder design

Simulation results

Leaf cell design
l


Future Improvements

Multiple error correction

Burst error handling

Low-power design

Better security systems


Conclusion

This project helps in understanding how Hamming Code improves data reliability by detecting and correcting errors during communication. It also gives basic knowledge about FPGA-based digital systems and error correction techniques.
