# QHack2022_project
 
### Team Name: 

ABOBA

### Project Description: 

Quantum chemistry applications of quantum computing have been of great interest recently. A fundamental task for them is to find ground and excited states of the molecules and other physical systems. There are several approaches to implement this search, with Variational Quantum Eigensolver (VQE) being one of the most interesting. This is an iterative process where, at each step, a sequence of parameterized quantum gates is applied to an initial state and the expected energy of the resulting state is measured. A classical algorithm uses the measurement results to adjust the gate parameters in an attempt to minimize the energy for the next measurement. However, running this process on near-term (NISQ) devices may be prohibitively costly for complicated structures. Using Quantum Approximate Optimization Algorithm (QAOA) demonstrated great efficiency on NISQ devices. This means the modification of VQE with QAOA can lead to better results for obtaining the energy spectrum of a complicated molecule, using today's quantum computers. 

In this project, I implement a QAOA routine to obtain excited states of several molecules and then compare the results and efficiency of an algorithm with existing results. Starting with "H-H" molecule, I will obtain spectrums of "LiH" and "CaH+", with the latter being a highly promising qubit-candidate for trapped-ion quantum computing realization. The project is highly inspired by the 500-points coding challenge in the quantum chemistry category.

### Source code: 

See repository.

### Resource Estimate: 

The main motivation for this project is to examine algorithm performance on the existing NISQ devices. This implies that it is necessary to compare results from simulation and real quantum computers. Moreover, simulating molecules with complicated structures, such as CaH, requires a sufficient number of qubits. I plan to use IonQ device, because of the full connectivity and high fidelity of operations. Since QAOA algorithm requires a sufficient number of layers, these advantages will help to reduce optimization mistakes. Furthermore, to evaluate the efficiency of the algorithm, the QAOA phase diagrams will be drawn, so that the most optimal parameters' set will be obtained. For this, a high number of computations is required, which will increase the cost drastically. With additional resources from AWS power-up, this task will be more achievable. 

### References:

Vladimir Kremenetski et al, Quantum Alternating Operator Ansatz (QAOA) Phase Diagrams and Applications for
Quantum Chemistry, arXiv:2108.13056 [quant-ph]

J. Pople, M. Head-Gordon, D. Fox, K. Raghavachari, and L. Curtiss, J. Chem. Phys. , 5622 (1989).

A. Peruzzo, J. McClean, P. Shadbolt, M.-H. Yung, X.-Q. Zhou, P. J. Love, A. Aspuru-Guzik, and J. L. O’Brien, Nature Communications 5, 4213 (2014)
