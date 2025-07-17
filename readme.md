
Surface Code in Stim
![alt text](https://img.shields.io/badge/Python-3.8+-blue.svg)

![alt text](https://img.shields.io/badge/License-Apache%202.0-blue.svg)

This repository contains a hands-on programming lab designed to construct, visualize, and simulate the surface code for quantum error correction using Google's high-performance quantum circuit simulator, Stim.

This lab is structured as a Jupyter Notebook that guides you through the process of building a complete surface code circuit from the ground up. We will implement the core logic in a separate Python file, surface_code.py, and use the notebook to test, visualize, and analyze the implementation.

🚀 Learning Objectives
By completing this lab, we will:

Understand Qubit Layout: Grasp a practical qubit indexing and coordinate system for the surface code.
Visualize Quantum Circuits: Use Stim's powerful visualization tools, like timeline-svg and timeslice-svg, to debug and understand complex circuit structures.
Build Stabilizer Circuits: Implement the precise gate ordering for parallel CNOT gates required for surface code stabilizer measurements.
Construct a Full Error-Correcting Circuit: Write Python code to generate a complete surface code circuit for any given distance and number of measurement rounds.
Implement a Noise Model: Add realistic, circuit-level depolarizing noise to your circuit to simulate a real-world quantum device.
Use Detectors and Observables: Correctly place DETECTOR and OBSERVABLE_INCLUDE instructions, which are essential for decoding and calculating the logical error rate.
Simulate and Analyze Performance: Use the sinter library to run high-speed simulations, plot logical vs. physical error rates, identify the error-correcting threshold, and project the performance for large-scale applications.

🛠️ Getting Started
Prerequisites
You need a Python environment with the following libraries installed:

stim
sinter
pymatching
matplotlib
numpy
scipy
jupyter
You can install all dependencies using pip:

Generated bash
pip install stim sinter pymatching matplotlib numpy scipy jupyter
Use code with caution.
Bash
Running the Lab
Clone the Repository:
Generated bash
git clone https://github.com/your-username/surface-code-in-stim.git
cd surface-code-in-stim
Use code with caution.
Bash
Start Jupyter:
Generated bash
jupyter notebook
Use code with caution.
Bash
Open the Notebook:
In the browser, open Surface code in Stim.ipynb.
Follow the Instructions:
Work through the notebook cells sequentially. The notebook will complete specific functions inside the surface_code.py file. The lab is broken down into manageable steps:
Understanding the qubit layout.
Building a lattice of CNOT gates.
Adding stabilizer measurements.
Implementing the initialization, rounds, and final measurement steps with the correct detectors.

📊 Simulation and Results
The final sections of the notebook are dedicated to simulating the performance of the surface code you've built. Using sinter, we will:

Find the Threshold: Run simulations across various code distances and physical error rates to find the "break-even" point where increasing the code's size begins to suppress logical errors.
<img src="https://i.imgur.com/gO0tA7M.png" alt="Logical Error per Round Plot" width="600"/>
Project Performance: Use the data from the simulations to create a projection of the code distance required to achieve a target logical error rate, such as surviving for a trillion rounds of operation.
<img src="https://i.imgur.com/GzB9T3y.png" alt="Performance Projection Plot" width="600"/>

🌟 Review
By the end of this lab, we will have moved from the abstract theory of the surface code to a concrete, working, and noisy implementation.

For more information on quantum error correction: 

https://quantum-journal.org/papers/q-2021-07-06-497/

https://github.com/quantumlib/Stim

https://github.com/quantumlib/Stim/blob/main/doc/gates.md

https://github.com/quantumlib/Stim/blob/main/doc/file_format_stim_circuit.md

