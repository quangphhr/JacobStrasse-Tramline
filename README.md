# JacobStraße-Tramline
An OvGU Simulation project, Summer semester 2018

## The goal
A clear reason to whether the city of Magdeburg should create a tram line at JacobStraße or not.

## Project map

>                    E1              E2                      E3
>                    |               |                       |
>S1--T1--S2--T2--S3--T3--S4--T4--S5--T5--S6--T6--S7--T7--S8--T8--S9
>    |       |               |               |       |
>    W1      W2              W3              W4      W5


## Current progress

* Base model with 5 sources of car input and 3 source of tram input (1 currently disable).
* Histogram data and chart of car's life span, both directions.
* Pedestrian traffic light at T3
* Both cars and trams are limit at 50 km/h

## Problem

* The windows 3D view can not be calibrated. A big blank area is display insted of fullscreen.  An error relates to OPEN GL is also generated after every simulation.  This problem might be because of the graphic card.
* The "Car dispose" block some time do not destroy the car.
* When there is not enough space (S1, T2, T7, T8), especially S1, cars all act strangely: do not stop at the traffic light, can not turn. Is there a work-around? because S1 is naturally short.
* Is there a way to prioritize 1 lane, especially inner lane, because the tram is deploy there and should have priority.
* Is there a way to prevent car changing lane while moving in the road (not at cross road, that can be configured)? 

## To be done

* Completion Input real data of traffic light, car input statistics.
* Run the model 1000 times, 12 hours each to calculate the confident interval of "car life span"
* Validation: Compare the average Life span of car traveling JacobStraße with the real value. Also queue length if possible
* Experiment:
  * Creating a tramline, experiment 1 & 2 lane for car.
  * Optimize the location of the tram station (Tram station is in the middle of the road, all cars will have to wait for the tram).
  * Increase the number of trams from 6/hour to (1+5)\*6/hour during emergency situation and observe the increase delay time.
