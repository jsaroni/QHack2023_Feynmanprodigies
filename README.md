# QHack2023_Feynman prodigies

We are trying to find the ground state of BeH2, so it is worth knowing more about its physical chemistry. In the
formation of BeH2, the 2s orbital of beryllium and the 1s orbitals of both hydrogen atoms combine to form two
molecular orbitals: a bonding molecular orbital and an antibonding molecular orbital. The molecule is linear, with a
bond angle of 180 degrees, and the two hydrogen atoms occupy the antibonding molecular orbital. The task is to find
the ground state energy of the molecule.
H|Φ〉 = EG |Φ〉 (1)
Knowing the ground state energy of a molecule can help predict its reactivity, chemical stability, and spectroscopic
properties. With this motivation, we employ different VQE (variational quantum eigensolver) methods.
VQE stands for Variational Quantum Eigensolver [2], which is a quantum algorithm designed to estimate the ground
state energy of a quantum system using quantum computers. The goal of VQE is to find the lowest energy state of
a molecule, which is important for understanding its chemical properties and behavior. The algorithm starts with
an initial guess for the wave function of the molecule and then uses a classical optimizer to adjust the parameters of
the wave function to minimize the energy. The adjusted wave function is then sent to the quantum computer, which
calculates the energy of the wave function. This process is repeated iteratively, with the classical optimizer updating
the wave function parameters and the quantum computer calculating the energy until the energy converges to the
ground state energy of the molecule.
We have the vanilla flavor VQE [3] method; then we explore the Tetris Adaptive VQE [4], and we finally worked with
the Adaptive VQE [5, 6] method, which gave us the best results.
