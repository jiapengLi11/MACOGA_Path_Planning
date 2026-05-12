# MACOGA Path Planning

![Python](https://img.shields.io/badge/Python-3.8-blue)
![ACO](https://img.shields.io/badge/Algorithm-ACO-orange)
![GA](https://img.shields.io/badge/Algorithm-GA-purple)
![Task](https://img.shields.io/badge/Task-Path%20Planning-green)

## Overview

This repository is a path-planning experiment that combines ant colony optimization and genetic algorithms, followed by path simplification.

## Preview

| Initial Environment | Final Comparison |
| --- | --- |
| ![env](results/01_initial_environment.png) | ![comparison](results/05_path_comparison.png) |

## Highlights

- hybrid ACO + GA path-planning pipeline
- path simplification as a final refinement stage
- saved visual outputs for each phase of the experiment

## Project Structure

- `main.py`: complete experiment pipeline and figure generation
- `environment.py`: grid environment definition
- `aco.py`: ant colony optimization stage
- `ga.py`: genetic algorithm stage
- `path_simplification.py`: path simplification logic
- `utils.py`: plotting and helper functions
- `results/`: generated comparison images

## Workflow

The default pipeline is:

1. build a `15 x 15` grid environment with obstacles
2. find an initial path using ACO
3. optimize the path using GA
4. simplify the optimized path
5. save plots for analysis

## Setup

The repository currently lists:

```text
Python 3.8
numpy==1.21.6
matplotlib==3.5.2
```

## Run

```bash
python main.py
```

## Notes

- The repository also contains a presentation file and a work-report directory.
- This project is best viewed as an experiment reproduction / verification repository rather than a packaged application.
