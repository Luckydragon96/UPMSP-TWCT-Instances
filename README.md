# UPMSP-TWCT Instances

This repository contains instances and results for the Unrelated Parallel Machine Scheduling Problem with minimizing the total weighted completion time (UPMSP-WCT). 

## Introduction

The Unrelated Parallel Machine Scheduling Problem with Time Windows and Sequence Dependent Setup Times (UPMSP-TWCT) is a classic problem in combinatorial optimization. In this problem, a set of jobs must be processed on a set of parallel machines, each with its own availability schedule. Each job has a processing time and a release date, and there are time windows during which the jobs must be completed. Additionally, there are setup times between certain pairs of jobs, which depend on the sequence in which they are processed.

## Contents

This repository contains the following:

- `instances/`: Directory containing instance files in a specific format.
- `README.md`: This README file providing an overview of the repository.

## Instance Format

Each instance file follows a specific format:

InstanceName
NumberOfJobs NumberOfMachines
ProcessingTimes
ReleaseDates
TimeWindows
SetupTimes

- `InstanceName`: Name of the instance.
- `NumberOfJobs`: Number of jobs in the instance.
- `NumberOfMachines`: Number of machines in the instance.
- `ProcessingTimes`: Matrix specifying the processing times of jobs on machines.
- `ReleaseDates`: Array specifying the release dates of jobs.
- `TimeWindows`: Matrix specifying the time windows during which jobs must be completed.
- `SetupTimes`: Matrix specifying the setup times between pairs of jobs.

## Usage

These instance files can be used for benchmarking algorithms and solving instances of the UPMSP-TWCT problem.

## Citation

If you use these instances in your research, please cite the following paper:

[Insert citation information here]

## License

This repository is licensed under the [insert license type here]. See the [LICENSE](LICENSE) file for details.
