# Quant-Search
Quantum Circuit Search Algorithm

## Overview

In this coding project you will implement Grover’s Search and apply your implementation to two different problem configurations. Use Qiskit methods to support examining and visualizing the quantum state at various algorithmic stages to observe the way the algorithm evolves the quantum state towards a final solution.

## Part 0: Background
Grover’s Search is a quantum algorithm for performing unstructured search that uses a technique for boosting the probability of the solution state and reducing the probability of non-solution states. 

After initialization, it uses a two-stage process. The first is an Oracle, which flips the sign of the amplitude of the solution state while leaving untouched the non-solution states. The second is a Diffuser, or amplitude amplification, that performs a reflection about the mean amplitude, thus increasing the amplitude of the solution state(s) and decreasing the amplitude(s) of the non-solution state(s) .

- Your algorithm will consist of the following major stages:

- Circuit initialization and application of initial set of H gates

- Oracle (customized for a particular solution state)

- Diffuser (generic across all solution configurations)

- Each pair of Oracle+Diffuser is referred to as “one execution of Grover’s”.

## Part 1: 2-qubit configuration
Run your implementation in a 2-qubit configuration, using a target state of |10>. 

Use the Operator(circuit).draw(“latex”) method to display the unitary matrix associated with just the Oracle  for this problem’s configuration. 

Incrementally set up your circuit to go through 3 iterations of Grover’s Search using the Oracle configured for this problem 

After each iteration #1, #2, and #3:
  
- Print the circuit

- Use the Statevector() method on your circuit to obtain and print the state vector 

- Plot the probability distribution (use plot_distribution())

- Plot the probability amplitudes (these may be either positive or negative) using either the qsphere or bar chart methods


## Part 2: 3-qubit configuration
Run your implementation in a 3-qubit configuration, using a target state of |110>. 

Use the Operator(circuit).draw(“latex”) method to display the unitary matrix associated with just the Oracle for this problem’s configuration. 

Incrementally set up your circuit to go through 5 iterations of Grover’s Search using the Oracle configured for this problem 
After each of the 5 iterations: 
- Print the circuit
- Use the Statevector() method on your circuit to obtain and print the state vector 
- Plot the probability distribution (use plot_distribution())
- Plot the probability amplitudes (these may be either positive or negative) using either the qsphere or bar chart methods

























