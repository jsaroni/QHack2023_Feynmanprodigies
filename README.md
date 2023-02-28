# QHack2023_Feynman prodigies


Finding the ground state of large molecules is a core problem in quantum chemistry and physics. In this project, we will compare the performance of different methodologies for finding the ground state of the molecule BeH2. We use a range of methods including orbital freezing, active space transformation, circuit cutting and knitting technique, and Adaptive VQE. We also use error mitigation including Twirled Readout Error eXtinction, Zero-Noise Extrapolation within qiskit runtime where we can also use Probabilistic Error Cancellation.

In final_submission.ipynb we describe the implementation of different the methodologies to find the ground state of the molecule BeH2, each with their own merits and drawbacks. The methods consider only single and double excitations. Some greatly simplify the model while sacrificing chemical accuracy while others use error mitigation more efficiently through qiskit runtime which works well with hybrid algorithms such as VQE.

We are trying to find the ground state of BeH2, so it is worth knowing more on its physical chemistry. Beryllium has chemical formula 1s2 2s2 and the two hydrogens 1s1 in electron configuration notation. When the molecule BeH2 is formed, the s orbitals from the two hydrogens hybridize with the p orbitals from beryllium to form two sp molecular orbital bonds that want to be as far away from each other as possible due to electron repulsion and this results in a linear molecule. We use the sto3g basis to approximate slater type orbitals.

The first method is based on a crude approximation, restricting the Hilbert space to an active space defined by unbonded electrons within the BeH2 molecule.
