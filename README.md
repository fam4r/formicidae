# formicidae

## Features

- supports multiple domain size (matrix size)
- computes average execution time (by running the program N times)
- computes speedup
- computes strong scaling
- computes weak scaling
- saves computation results into CSV files (easy to plot!)
- verbose logging

## Usage

Run `./util/hpc-perf-evaluation.py` for OpenMP source codes.

Run `./util/hpc-perf-evaluation-cuda.py` for CUDA source codes.

Results will be available in the `data` folder as CSV files.

## Motivation

Made for problems involving matrixes, but built for general-purpose uses.

Program timings **must** be managed and printed by the program itself, since a
wrapper script like that one cannot separately consider the serial and the
parallel portions of the execution time.
