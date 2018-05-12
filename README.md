# JacobStraße-Tramline
An OvGU Simulation project, Summer semester 2018

## The goal
A clear reason to whether the city of Magdeburg should create a tram line at JacobStraße or not.

## Current progress
* Base model with 4 big cross road, 4 sources of car input
* Histogram data and chart of car's life span, both directions.
* No pedestrial yet.

## Problem

* The windows 3D view can not be calibrated. A big blank area is display insted of fullscreen.  An error relates to OPEN GL is also generated after every simulation.  This problem might be because of the graphic card.
* The "Car dispose" block some time do not destroy the car.
* The "Out way not found" port of the "Car move to" doesn't work most of the time.  A work-around is using for now

## To be done

* Completion Input real data of traffic light, turning probability, car input statistics.
* Validation: Compare the average Life span of car traveling JacobStraße with the real value.
* Experiment:
  * Creating a tramline, the JacobStraße will be narrowed down to 1 lane each direction.
  * Optimize the location of the tram station (Tram station is in the middle of the road, all cars will have to wait for the tram).
  * Increase the number of trams from 6/hour to (1+5)\*6/hour during emergency situation and observe the increase delay time.
