# BandPass_Filter
I implemented a BandPass Filter of 2nd Order into simulink by using Analog components : Resistors and Capacitors.

To achieve this goal, I started by implementing the LowPass and HighPass filters separately and ended up adding an amplifier to amplify my signal.

BandPass Filter Model into simulink : 

![BandPass_Filter_Simulink_Model](https://user-images.githubusercontent.com/43390471/55465519-9831d400-55fd-11e9-8257-1c39bace32e2.png)

So, by Cascading the HighPass and LowPass filters together I obtain a BandPass Filter.

The range of BandPass filter = [fc1 , fc2]

fc1 : Cutoff frequency of HighPass filter.
fc2 : Cutoff frequency of LowPass filter.

fc1 = 1/(2*pi*R1*C1)
fc2 = 1/(2*pi*R2*C2)

In this example I have chosen fc1 = 16Khz and fc2 = 24 Khz.

A : Gain = 1+(R4/R3)

Digram Bode : 

![Bode_Diagram_And_3db_Values](https://user-images.githubusercontent.com/43390471/55466112-d24fa580-55fe-11e9-9c9d-7f81c5515157.png)

