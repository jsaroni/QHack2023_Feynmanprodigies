# QHack2023_Feynman prodigies


Introduction 


We are trying to find the ground state of BeH2, so it is worth knowing more about its physical chemistry. In the
formation of BeH2, the 2s orbital of beryllium and the 1s orbitals of both hydrogen atoms combine to form two
molecular orbitals: a bonding molecular orbital and an antibonding molecular orbital. The molecule is linear, with a
bond angle of 180 degrees, and the two hydrogen atoms occupy the antibonding molecular orbital. The task is to find
the ground state energy of the molecule.
H|Φ〉 = EG |Φ〉 (1)
Knowing the ground state energy of a molecule can help predict its reactivity, chemical stability, and spectroscopic
properties. With this motivation, we employ different VQE (variational quantum eigensolver) methods.
VQE stands for Variational Quantum Eigensolver, which is a quantum algorithm designed to estimate the ground
state energy of a quantum system using quantum computers. The goal of VQE is to find the lowest energy state of
a molecule, which is important for understanding its chemical properties and behavior. The algorithm starts with
an initial guess for the wave function of the molecule and then uses a classical optimizer to adjust the parameters of
the wave function to minimize the energy. The adjusted wave function is then sent to the quantum computer, which
calculates the energy of the wave function. This process is repeated iteratively, with the classical optimizer updating
the wave function parameters and the quantum computer calculating the energy until the energy converges to the
ground state energy of the molecule.
We have the vanilla flavor VQE [3] method; then we explore the Tetris Adaptive VQE [4], and we finally worked with
the Adaptive VQE [5, 6] method, which gave us the best results.


Circuit knitting 


Circuit knitting is a technique in quantum computing that involves combining multiple quantum circuits into a larger,
more complex circuit. The idea behind circuit knitting is to use smaller, more specialized circuits as building blocks,
which can be combined and stitched together to create larger, more powerful circuits for solving complex problems.
Overall, circuit knitting is a powerful technique in quantum computing that can help researchers tackle some of the
most challenging problems in the field. It is a testament to the versatility and modularity of quantum circuits, and it
has the potential to enable new breakthroughs in quantum technology.


Entanglement forging


Entanglement forging refers to a hypothetical process in which two parties can create a shared quantum state
without actually having access to an entangled pair of qubits. This is accomplished through a combination of quan-
tum operations and classical communication and would represent a significant breakthrough in the field of quantum
information processing. The basic idea behind entanglement forging is to start with two separable qubits (i.e., qubits
that are not entangled with each other) and then use a series of quantum gates and measurements to create a new
state that is entangled.
Entanglement forging takes a generic circuit that operates on the combined system of the spin-up and spin-down
halves and splits it into smaller circuits that only operate on one half at a time. In other words, the entanglement
forging technique takes a circuit operating on 2N qubits and separates that circuit into two N-qubit halves.


Zero Noise Extrapolation

Zero noise extrapolation (ZNE) is a technique in quantum computing that can improve the accuracy of quantum al-
gorithms by extrapolating the results of noisy quantum circuits to the limit of zero noise.
In a noisy quantum circuit, the presence of unwanted noise can cause errors in the computation, which can reduce
the accuracy of the results. ZNE aims to mitigate this problem by extrapolating the noisy results to the limit of zero
noise, where the true value of the computation can be obtained without any errors.
One advantage of the ZNE technique is that it can be applied to any quantum algorithm, regardless of its specific
structure or purpose. Moreover, ZNE can be combined with other noise mitigation techniques, such as error correction
and error suppression, to further improve the accuracy and reliability of quantum computations.


Twirled Readout Error eXtinction

TREX (Twirled Readout Error eXtinction) is an error mitigation technique in quantum computing that combines
twirled readout with excitations to improve the accuracy of quantum measurements. The twirled readout is a tech-
nique that involves applying a random unitary transformation to the final state of a quantum circuit before measuring
it. The idea behind this technique is to randomly rotate the state space in a way that cancels out certain types of
noise, such as systematic errors in the measurement process.
TREX has been shown to be effective in a variety of quantum computing applications, including quantum chemistry
simulations, optimization problems, and machine learning tasks. It is a promising technique for overcoming the
limitations of noisy, near-term quantum devices and enabling the development of more accurate and reliable quantum
algorithms.


