# EX 02- EXECUTION OF TIMER OPERATIONS USING LADDER LOGIC PROGRAMMING


 #### NAME :CHANDRU P
 #### REGISTER NUMBER :212223110007
 #### DEPARTMENT:CSE(IOT)
 #### YEAR :3rd

 
# Aim:
To understand and implement timer operations in a PLC using ladder logic and verify the output for different types of timers (ON-delay, OFF-delay, and Retentive timers).

# Apparatus Required:
Programmable Logic Controller (PLC) - A PLC that supports timer functions.
PLC Programming Software - Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System - For programming and simulating the PLC ladder logic.
Input Devices - Push buttons or switches for triggering the timer operations.
Output Devices - LEDs or any other indicators to visualize the timer output.
Wires and Connectors - For interfacing input/output devices with the PLC.
Power Supply - Appropriate power supply for the PLC and peripherals.
# Theory:
Timers in PLCs are used to introduce delays in control processes. They are fundamental in operations where the timing of events is crucial, 
such as starting a motor after a delay, turning off a light after a specified time, or maintaining a state for a fixed duration.

# Types of Timers:
 1. ON-Delay Timer (TON)
Functionality:

The ON-delay timer starts timing when the input condition becomes TRUE (ON).
After the preset time has elapsed, the timer output becomes TRUE (ON).
If the input condition turns FALSE (OFF) before the timer completes, the timer resets, and the output remains FALSE.
2. OFF-Delay Timer (TOF)
Functionality:

The OFF-delay timer starts timing when the input condition turns FALSE (OFF).
The timer output remains TRUE (ON) during the preset delay time and then turns FALSE (OFF) after the time has elapsed.
If the input condition becomes TRUE (ON) during the timing process, the timer resets.
3. Retentive ON-Delay Timer (RTO)
Functionality:

The Retentive ON-delay timer accumulates time as long as the input condition is TRUE (ON).
The accumulated time is retained even if the input condition turns FALSE (OFF).
The timer continues from the accumulated time when the input condition becomes TRUE again.
A separate reset input is usually provided to clear the accumulated time.
4. Pulse Timer (TP or TONR)
Functionality:

The Pulse Timer generates an output pulse of a specific duration when the input condition becomes TRUE (ON).
The output remains TRUE for the preset duration, regardless of the input state.
5. Timer-On Interval (TONI)
Functionality:

The Timer-On Interval is a variation of the ON-delay timer but is used to measure the time interval while the input is TRUE (ON).
The timer counts up as long as the input is TRUE and resets when the input turns FALSE.

 
# Procedure:
Setup the PLC Programming Environment:

Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Timers:

Implement the ON-delay timer (TON) by creating a rung with an input (e.g., a push button) linked to a TON instruction. Set the preset time (e.g., 5 seconds).
Implement the OFF-delay timer (TOF) by creating a rung with an input linked to a TOF instruction. Set the preset time (e.g., 5 seconds).
Implement the Retentive Timer (RTO) by creating a rung with an input linked to an RTO instruction. Set the preset time and enable an additional rung to reset the timer when required.
Simulate the Ladder Logic:

Run the simulation in the PLC software.
Test the ON-delay timer by pressing the input button and observing the delay before the output is activated.
Test the OFF-delay timer by deactivating the input and observing the delay before the output turns off.
Test the Retentive Timer by toggling the input on and off, observing how the accumulated time is retained.
Download and Execute:

Download the ladder logic program to the PLC if available and run it.
Test the timers with the physical push buttons and observe the LEDs or other output devices.
#   Outputs:
ON-Delay Timer: The output LED or indicator should turn on after a specified delay (e.g., 5 seconds) once the input is activated.
OFF-Delay Timer: The output should remain on for the specified delay after the input is deactivated, and then it should turn off.
Retentive Timer: The output should turn on after the accumulated time reaches the preset value, and it should retain the accumulated time even if the input is turned off.


# Simulation Screenshots 

<img width="602" height="498" alt="Screenshot 2026-02-08 183820" src="https://github.com/user-attachments/assets/902fc7be-b6a9-4253-a335-12cdb8765e5e" />

<img width="575" height="631" alt="Screenshot 2026-02-08 183838" src="https://github.com/user-attachments/assets/e5366939-89e7-4f94-857b-2e81edb80070" />

<img width="841" height="443" alt="Screenshot 2026-02-08 183859" src="https://github.com/user-attachments/assets/dcd9485a-aad9-4bc5-aa6e-767279b72ecb" />

<img width="696" height="640" alt="Screenshot 2026-02-08 184439" src="https://github.com/user-attachments/assets/0f969f24-0513-49ec-85b5-47d8d33086a2" />

<img width="629" height="576" alt="Screenshot 2026-02-08 184449" src="https://github.com/user-attachments/assets/af8a1257-e7d0-4f99-98ab-4e4932bc827b" />

<img width="785" height="237" alt="Screenshot 2026-02-08 184457" src="https://github.com/user-attachments/assets/a8aeabc8-683c-4f50-9ecd-bde0034e10e3" />

<img width="1919" height="1079" alt="Screenshot 2026-02-08 184511" src="https://github.com/user-attachments/assets/a605fb19-e108-417c-954a-487a3ad2275e" />


<img width="1900" height="1079" alt="Screenshot 2026-02-08 185627" src="https://github.com/user-attachments/assets/bb132853-c7dd-4a95-b303-01a0b2bf79cb" />



















# Results:
The ladder logic programs for ON-delay, OFF-delay, and Retentive timers were successfully implemented and tested.
The observed outputs matched the expected behavior of each type of timer, demonstrating the correct functioning of timer operations in PLC ladder logic.
The experiment confirms the practical application of timers in controlling process sequences and managing time-dependent operations in industrial automation.
