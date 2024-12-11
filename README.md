# Truss Optimization in 3D

## Overview
This repository contains materials related to the "Truss Optimization in 3D" project, presented as part of the ME 260 course on Structural Optimization: Size, Shape, and Topology. The project focuses on optimizing 3D truss structures to maximize stiffness (minimize mean compliance) while ensuring efficient material usage within a fixed material volume constraint.

## Problem Statement
The goal of this project is to:
- Optimize the material distribution across truss elements to maximize stiffness.
- Ensure the structure satisfies the given constraints, including a fixed material volume.

## Motivation
Efficient material usage is critical for lightweight and high-performance structural designs. Optimizing 3D trusses for stiffness has applications in aerospace, civil, and mechanical engineering, contributing to sustainable and cost-effective design practices.

## Methodology

### Algorithm Steps
1. **Initialization:**
   - Set up initial areas for truss elements.
   - Define parameters like maximum iterations, tolerance, and tuning parameter (β).
2. **Strain Energy Computation:**
   - Perform finite element analysis to compute strain energy for all truss elements.
   - Calculate strain energy density based on stiffness, volume, and material properties.
3. **Area Update Using Optimality Criteria:**
   - Compute the Lagrange multiplier (Λ) to satisfy volume constraints.
   - Update areas of truss elements iteratively to adhere to the constraints.
4. **Convergence Check:**
   - Evaluate convergence by monitoring changes in area values across iterations.
   - Terminate the optimization process when the maximum change is below a set tolerance.
5. **Finalization:**
   - Filter out elements with negligible areas.
   - Prepare the optimized structure for visualization and post-processing.

### Implementation Highlights
- Transformation matrices were employed for converting between 2D and 3D representations.
- Overlapping elements in the ground structure were removed to enhance optimization efficiency.

### Example Structures
Several examples were tested and optimized to validate the algorithm's efficacy.

## Results
- Successfully optimized 3D truss structures for maximum stiffness.
- Achieved efficient material distribution using the optimality criteria method.
- Demonstrated improvements in design for various example truss structures.

## Files
- **`Truss Optimization in 3D.pptx`**: The presentation summarizing the project methodology, examples, and results.
- Additional files and scripts may be added for implementation details and supplementary data.

## Authors
- **Gunturu Akhil Sai Krishna Mouli (23166)**
- **Jayhind Chauhan (22737)**
- 
## Acknowledgments
- Instructor: Prof. G. K. Ananthasuresh
- ME 260: Structural Optimization - Size, Shape, and Topology

## License
This repository is shared under the MIT License. See `LICENSE` for details.

