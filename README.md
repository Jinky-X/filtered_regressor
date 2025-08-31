# Acceleration-Free Analytical Regressor Filtering simulation

This repository contains simulation and test code for filtered regression algorithms of AF-ARF.

## Dependencies

- [ROS](https://www.ros.org/)
- [Eigen](https://eigen.tuxfamily.org/)
- [Pinocchio](https://gepettoweb.laas.fr/doc/stack-of-tasks/pinocchio/master/doxygen-html/index.html)

## Usage

To start the simulation, run:

```bash
roslaunch filter_regressor sim.launch use_analytic:=1 # use analytic regressor

roslaunch filter_regressor sim.launch use_analytic:=0 # use pinocchio regressor
```

## Description

This project supports two regressor computation methods: an analytic approach with hand-derived equations, and the Pinocchio library for automatic model-based regressor computation. Select the method via the `use_analytic` parameter.
