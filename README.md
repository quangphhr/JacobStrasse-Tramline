
# JacobStraße-Tramline
An OvGU Simulation project, Summer semester 2018

## The goal
A clear reason to whether the city of Magdeburg should create a tram line at JacobStraße or not.

## Project map
<pre>
                    E1              E2                      E3
                    |               |                       |
S1--T1--S2--T2--S3--T3--S4--T4--S5--T5--S6--T6--S7--T7--S8--T8--S9
    |       |               |               |       |
    W1      W2              W3              W4      W5
</pre>

## Current progress

* Base model with 5 sources of car input.  Cars are generated using normal distribution with min/max limit.
* Base model with 3 sources of tram input with fixed rate.
* S1 is made to be stretched out of the map to have enough space for the car to function normally.
* Pedestrian traffic light at T3
* Both cars and trams are limit at 50 km/h
* Histogram data and chart of car's life span, both directions.
* Code for counting queue length at E3 and S7 (northward) at T6 and T8.
* Validation successfully with real world data (Delay time and 2 queue-lengths)
* 4 Experiments

## Problem

* The windows 3D view can not be calibrated. A big blank area is display insted of fullscreen.  An error relates to OPEN GL is also generated after every simulation.  This problem might be because of the graphic card.
* Prioritization of 1 lane, especially inner lane for Tram.
* No Experiment on "Emergency Situation" Yet

## Recommendation

* The traffic condition will mostly stays the same with the tram line built.
* To build or not to build: why not.

