# UPMSP-TWCT Benchmark

This repository contains instances and results for the Unrelated Parallel Machine Scheduling Problem with minimizing the total weighted completion time (UPMSP-WCT). 

## Introduction

The Unrelated Parallel Machine Scheduling Problem (UPMSP) is a fundamental challenge in combinatorial optimization and has been extensively researched for decades. It has widespread applications in production scheduling, computing service scheduling, TV advertisement scheduling, and resource allocation in workforce planning, to name a few. 

The UPMSP is given a set $N$ of $n$ independent jobs that must be scheduled on a set $M$ of $m$ unrelated parallel machines. Each job $j \in N$, is defined by $m$ processing times $p_{jk}$, $\forall k \in M$,  and a weight $w_j$. Importantly, the processing times $p_{jk}$ are *unrelated*, i.e., they are arbitrary and do not possess any characteristic related to the machines. Each machine can handle only one job at a time, and a single machine must process each job without interruptions or preemption. Let $C_j$ be the completion time of job $j \in N$ in a solution to the problem. The objective is to find a schedule minimizing the total weighted completion time computed as $\sum_{j \in N}w_jC_j$.

## Contents

This repository contains the following:

- `UPMSP-WCT Instances/`: Directory containing instance files in a specific format.
- `UPMSP-WCT Results/`: Directory containing results solved by our Branch-Price-and-Cut (BPC) method in a specific format.
- `BP Results/`: Directory containing results solved by our Branch-and-Price (BP) method in a specific format.
- `BSSU Results/`: Directory containing results solved by other BPC method in a specific format.
- `Effectiveness of the Main Components/`: Directory containing results on effectiveness of the main components of our BPC method in a specific format.
- `README.md`: This README file providing an overview of the repository.

For more details on BPC, BP, and BSSU algorithms stay tuned to the papers we are submitting.

## Usage

The proposed BPC algorithm is implemented in C\# with ILOG CPLEX 12.8 serving as the LP solver. All tests are conducted on a computer with a 2.50 GHz IntelCoreTM i9-12900H processor running Microsoft Windows 11 and equipped with 16.0 GB of RAM. A time limit of one hour was imposed for each execution of the BPC algorithm.

These instance files can be used for benchmarking algorithms and solving instances of the UPMSP-TWCT problem. 

## Citation

If you use these instances in your research, please cite the following paper:

[Insert citation information here]

Our paper with the title "An Exact Branch-Price-and-Cut Algorithm for the Unrelated Parallel Machine Scheduling Problem" and authors "Yang Yu, Xiaolong Li, Roberto Baldacci, Wei Sun, Jiafu Tang, Zhiqiao Wu, and Han Zhu" is being submitted to ***INFORMS Journal on Computing***.

## License

This repository is licensed under the [insert license type here]. See the [LICENSE](LICENSE) file for details.
