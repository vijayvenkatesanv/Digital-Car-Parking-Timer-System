# Power Supply Module
The system operates on a 5V regulated power supply, ensuring stable operation for all digital components. Voltage regulators maintain consistent power delivery to counters, logic gates, and display drivers.

# Parking Slot Detection and Timer Activation
Each of the four parking slots is equipped with a digital logic-based detection mechanism. When a vehicle occupies a slot, the corresponding mod-5 and mod-9 counters begin counting, tracking time in minutes and hours.

# Counter Module (Time Measurement)
Each parking slot features:

Two mod-5 counters (for counting units place of minutes and hours).

Two mod-9 counters (for counting tens place of minutes and hours).
These counters ensure accurate real-time tracking of the vehicle’s duration in the slot.

# Multiplexing and Display Module
A multiplexed 7-segment display system allows a single display to show time for multiple slots.

Two displays for minutes and two for hours.

Multiplexers (14 in total) control which slot’s timing is displayed at a given moment.

BCD to 7-segment decoders (74LS47) convert the counter outputs into a format suitable for display.

# Control and Reset Module
Each slot has an individual reset button to manually clear the counter when needed.

Logic ICs (7404, 7408, 7432, 74HC393, 74LS47) handle display switching, counting operations, and control logic.

# Simulation and Testing
The circuit is designed and simulated in Proteus to verify its accuracy and efficiency before real-world implementation.

Ensures all logic gates, counters, and multiplexers work as expected in tracking and displaying parking duration.

This system offers a cost-effective and reliable method for monitoring parking duration using only digital logic components, eliminating the need for microcontrollers.
