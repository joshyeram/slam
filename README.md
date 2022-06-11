# Shot Gun Spread Filtering and Kalman Filtering #

## Kalman Filtering ##
Givne actions and observartion data set, the agent can be self localized better in comparison to just using the observations.
<p align="center">
  <img src="https://github.com/joshyeram/slam/blob/main/distrib/kf.png", width="600"/>
</p>
Given just the observations, the red trajectory is not smooth and seems as if the robot is oscillating. In conjunction with the action data set, the path is actual path is smoothed out.

## Shot Gun Spread Filtering ##
Instead of implementing the known particle filtering model, a new filtering method was developed: Shot Gun Spread Filtering. Given an action (direction and velocity) and landmark observations, we can determine the best-predicted location of the robot and normalize it along with the observation point. 
