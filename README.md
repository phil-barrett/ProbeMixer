# ProbeMixer

ProbeMixer is designed to allow multiple simple switches or NPN current sinking sensors that are Normally Open or Normally Closed to share a single probe input line. It is also designed to support 5, 12 or 24V power and have separate but combinable power zones for input and output.

ProbeMixer support 4 input signals: A touch probe, a 3D probe, a tool setter probe and a tool setter overtravel signal.  The first 3 are combined into a single probe output signal that behaves as an N.O. signal.  N.C. input signals are inverted via a configuration jumper header.  The tool setter overtravel input is output on a separate line to allow use as an emergency stop input.

ProbeMixer is not designed to support PNP sensors.

![ProbeMixer V0.91](https://github.com/phil-barrett/ProbeMixer/blob/main/Photos/probemixer%20V091.jpg)

## Aug 29, 2026

Created DIN Rail brackets (via my parametric DIN Rail generator) for ProbeMixer.  Fixed dimension errors on mounting holes. Uploaded new photos/renderings.

![DIN Rail brackets w/ProbeMixer](https://github.com/phil-barrett/ProbeMixer/blob/main/Photos/ProbeMixer%20V0.91%20wDIN%20Rail%20Brackets.jpeg)

## Power options for ProbeMixer

Probemixer was designed to support multiple power options.  The input and output sections can be powered separately. It supports 5V, 12V and 24V on either. Typically, The input section will be powered to match the probe peripherals and the output section powered to match the input of the CNC controller board.

For example, using ProbeMixer with a 5V device like an Arduino, one would use 5V for the output section and power the input section with the voltage recommended for the probes.

Note, that 5V on the input section requires closing the solder jumpers to reduce the resistance for the opto-isolators.  This creates some risks. Specifically, a ProbeMixer set up for 5V inputs will not tolerate 12 or 24V power. That WILL damage the board. Fortunately, there are few powered probes that require 5V.

## Aug 28, 2026

V0.91 sent off for small test build. Expect boards back in 7-10 days.
