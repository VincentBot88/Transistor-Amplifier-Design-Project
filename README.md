# Transistor Amplifier Design Project

Designed, simulated, analyzed, implemented, and tested a single-supply, multistage, inverting transistor amplifier.  
Conducted calculations for resistance, capacitance, and biasing, and verified results through simulations.

## Introduction

This project involved designing and verifying a single-supply, multistage inverting transistor amplifier based on the provided specifications:

- **Power supply**: +10V relative to ground
- **Quiescent current** drawn from the power supply: no larger than 10 mA
- **No-load voltage gain** (at 1 kHz): |A_vo| = 50 (± 10%)
- **Maximum no-load output voltage swing** (at 1 kHz): no smaller than 8 V peak-to-peak
- **Loaded voltage gain** (at 1 kHz and with R_L = 1 kΩ): no smaller than 90% of the no-load voltage gain
- **Maximum loaded output voltage swing** (at 1 kHz and R_L = 1 kΩ): no smaller than 4 V peak-to-peak
- **Input resistance** (at 1 kHz): no smaller than 20 kΩ
- **Amplifier type**: inverting or non-inverting
- **Frequency response**: 20 Hz to 50 kHz (−3dB response)
- **Type of transistors**: BJT
- **Number of transistors (stages)**: no more than 3
- **Resistances permitted**: values smaller than 220 kΩ from the E24 series
- **Capacitors permitted**: 0.1 μF, 1.0 μF, 2.2 μF, 4.7 μF, 10 μF, 47 μF, 100 μF, 220 μF
- **Other components** (BJTs, diodes, Zener diodes, etc.): only from your ELE404 lab kit

## Circuit Design Justification

The choice of a **CE-CC amplifier configuration** is justified by its advantages in meeting the project specifications and design requirements:

- The **common emitter (CE) stage** provides a **high voltage gain** of 50, suitable for amplifying weak signals while maintaining stability.
- The CE configuration offers a **relatively high input impedance**, ensuring efficient signal coupling and compatibility with signal sources.
- The **common collector (CC) stage** (emitter follower) serves to **buffer the output** of the CE stage, minimizing loading effects of the 1 kΩ resistor on the CE stage.
- The CC stage allows for **high input impedance** and **low output impedance**, conducive to achieving the desired voltage swings and amplifier performance.
- The CC stage provides **unity voltage gain**, ensuring that the output voltage tracks the input voltage while offering **high current gain**.
- This configuration facilitates **AC coupling** between amplifier stages, as required by the project specifications.

In summary, the **CE-CC amplifier configuration** combines the **high voltage gain** of the CE stage with the **buffering capabilities** of the CC stage, offering an optimal design for the given amplifier requirements.
