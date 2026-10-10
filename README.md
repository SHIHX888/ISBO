# ISBO: An Improved Status-Based Optimization Framework for Global Optimization Problems and UAV Obstacle Avoidance Trajectory Planning

## 1. Project Overview

This repository provides the MATLAB implementation and experimental materials associated with the research project entitled **"ISBO: An Improved Status-Based Optimization Framework for Global Optimization Problems and UAV Obstacle Avoidance Trajectory Planning."**

The project investigates the optimization performance of the Improved Status-Based Optimizer (ISBO) for numerical optimization problems and unmanned aerial vehicle (UAV) obstacle avoidance trajectory planning.

The repository is intended to support research reproducibility by providing the experimental implementations used for benchmark evaluation, exploration and exploitation analysis, and UAV trajectory planning.

## 2. Repository Structure

The repository contains three experimental packages and this documentation file.

```text
ISBO/
│
├── CEC.7z
│   └── Benchmark optimization experiments
│
├── Exploration and development.7z
│   └── Exploration and exploitation analysis
│
├── UAV.7z
│   └── UAV obstacle avoidance trajectory planning
│
└── README.md
```

The experimental materials are organized as follows:

- **CEC.7z:** Contains materials for evaluating optimization performance on the CEC benchmark functions.
- **Exploration and development.7z:** Contains materials related to the analysis of exploration and exploitation behavior.
- **UAV.7z:** Contains materials for evaluating the algorithm in UAV obstacle avoidance trajectory planning.

The archive files must be extracted before running the corresponding experiments.

## 3. Algorithm Description

ISBO is an improved optimization framework developed to address global optimization problems and UAV trajectory planning tasks.

The algorithm is evaluated from the following perspectives:

1. **Numerical optimization:** Assessment of optimization accuracy and convergence behavior on benchmark test functions.
2. **Exploration and exploitation:** Investigation of the search behavior of the algorithm during the optimization process.
3. **Practical application:** Evaluation of the applicability of ISBO to UAV obstacle avoidance trajectory planning.

These experiments provide a basis for evaluating the effectiveness and applicability of ISBO across different optimization scenarios.

For the mathematical formulation, implementation details, and algorithmic design, please refer to the associated research manuscript.

## 4. Benchmark Functions and Data Information

### 4.1 CEC2017 Benchmark Suite

The CEC2017 benchmark suite is employed to evaluate the global optimization performance of ISBO.

The experiments associated with this project consider the 30-dimensional CEC2017 benchmark functions.

Reference implementation:

https://github.com/P-N-Suganthan/CEC2017

### 4.2 CEC2022 Benchmark Suite

The CEC2022 benchmark suite is used to further investigate the optimization performance of ISBO under different problem dimensions.

The experiments consider two dimensional settings:

- 10 dimensions (10D)
- 20 dimensions (20D)

Reference implementation:

https://www.mathworks.com/matlabcentral/fileexchange/157611-cec2022

### 4.3 UAV Trajectory Planning

The UAV experiments are designed to evaluate the applicability of ISBO to obstacle avoidance trajectory planning.

The corresponding MATLAB implementation is provided in `UAV.7z`.

These experiments investigate the ability of the optimization algorithm to identify feasible UAV trajectories in an environment containing obstacles.

## 5. Software Requirements

The experimental code was developed using the following software environment:

- **Programming language:** MATLAB
- **Development version:** MATLAB R2023a
- **Operating system:** A system compatible with MATLAB R2023a
- **Additional requirements:** The relevant benchmark function implementations and supporting MATLAB files must be available on the MATLAB search path.

The use of MATLAB R2023a is recommended to maintain consistency with the original development environment.

## 6. Installation and Usage Instructions

### Step 1: Download the Repository

Clone the repository using Git:

```bash
git clone https://github.com/SHIHX888/ISBO.git
```

Alternatively, download the repository directly from GitHub using **Code → Download ZIP**.

### Step 2: Extract the Experimental Files

Extract the following archives using software supporting the `.7z` format:

```text
CEC.7z
Exploration and development.7z
UAV.7z
```

Each archive contains the materials corresponding to a different experimental component.

### Step 3: Open MATLAB

Launch MATLAB R2023a and navigate to the directory containing the extracted experimental files.

Make sure that the required functions and supporting files are accessible from the MATLAB environment.

If necessary, add the experiment folder and its subfolders to the MATLAB search path:

```matlab
addpath(genpath(pwd));
```

### Step 4: Run the Experiments

Locate the main experimental script in the corresponding extracted folder.

For experimental folders containing a `main.m` entry script, execute:

```matlab
run('main.m');
```

The benchmark experiments, exploration and exploitation analysis, and UAV trajectory planning experiments should be executed separately from their corresponding directories.

Before execution, users should check the experimental settings and file paths defined in each main script.

### Step 5: Examine the Results

The MATLAB programs can be used to reproduce the experimental procedures associated with the study.

Depending on the experiment, the outputs may include:

- Optimization fitness values
- Algorithm convergence behavior
- Exploration and exploitation characteristics
- UAV obstacle avoidance trajectories
- Numerical and graphical experimental results

The exact output files and figures depend on the implementation of each experimental script.

## 7. Experimental Reproducibility

The repository provides the experimental materials associated with the evaluation of ISBO.

To facilitate reproducibility, users are encouraged to maintain experimental settings consistent with those reported in the manuscript, including:

- Population size
- Maximum number of iterations or fitness evaluations
- Problem dimensionality
- Number of independent runs
- Benchmark function selection
- UAV environment and obstacle configurations

Because ISBO is a stochastic optimization algorithm, numerical results may vary between independent executions.

For fair algorithm comparisons, the same experimental conditions should be used for all compared methods.

## 8. Citation

If you use the ISBO implementation or experimental materials in your research, please cite the associated paper:

**ISBO: An Improved Status-Based Optimization Framework for Global Optimization Problems and UAV Obstacle Avoidance Trajectory Planning.**

The complete bibliographic information should be added when the paper's publication details become available.

The original benchmark implementations should also be acknowledged when applicable.

## 9. Code Availability and Usage

The source code and experimental materials are provided for academic research and reproducibility purposes.

Users should appropriately acknowledge the associated research work and the original sources of any third-party benchmark implementations.

No separate software license is specified in this repository. Redistribution and modification permissions should therefore not be assumed without authorization.

## 10. Contact and Feedback

For questions about the implementation, experimental settings, or reproducibility of the results, please use the GitHub repository's issue-tracking functionality:

https://github.com/SHIHX888/ISBO/issues
