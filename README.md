# ProbeMixer

ProbeMixer is designed to allow multiple simple switches or NPN current sinking sensors that are Normally Open or Normally Closed to share a single probe input line. It is also designed to support 5, 12 or 24V power and have separate power zones for input and output.

ProbeMixer support 4 inputs: A touch probe, a 3D Probe, a tool setter probe and a tool setter overtravel signal.  The first 3 are combined into a single probe output signal that behaves as an N.O. signal.  N.C. input signals are inverted via a configuration jumper header.  The tool setter overtravel input is output on a separate line to allow use as an emergency stop input.

ProbeMixer is not designed to support PNP sensors.
