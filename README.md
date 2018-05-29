
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
* 3 sources of tram input with fixed rate (1 currently disable).
* S1 is made to be stretched out of the map to have enough space for the car to function normally.
* Pedestrian traffic light at T3
* Both cars and trams are limit at 50 km/h
* Histogram data and chart of car's life span, both directions.
* Code for counting queue length at E3 and S7 (northward) at T6 and T8.
* **For Validation** all car sources are changed to generate normal hour car for 1 hour, then rush hour car rate.  The validation experiment runs for 2 hour only.


## Problem

* The windows 3D view can not be calibrated. A big blank area is display insted of fullscreen.  An error relates to OPEN GL is also generated after every simulation.  This problem might be because of the graphic card.
* When there is no lane connector (to turn for example), the model generates error instead of pushing the car to "out way not found".
![Error1](https://github.com/quangphhr/JacobStrasse-Tramline/blob/master/Material/Out%20way%20not%20found.png "Out way not found")
* Is there a way to prioritize 1 lane, especially inner lane, because the tram is deploy there and should have priority.


## To do

* Adapt the source for pedestrial traffic light at T3 *(Wait for Data Master)*.
* Run the model 1000 times, 12 hours each to calculate the confident interval of "car life span"
* Validation: Compare the average Life span of car traveling JacobStraße with the real value. Also queue length if possible
* Experiment:
  * Creating a tramline, experiment 1 & 2 lane for car.
  * Optimize the location of the tram station (Tram station is in the middle of the road, all cars will have to wait for the tram).
  * Increase the number of trams from 6/hour to (1+5)\*6/hour during emergency situation and observe the increase delay time.
