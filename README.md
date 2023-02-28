# QHack2023_Feynmanprodigies


Finding the ground state of large molecules is a core problem in quantum chemistry and physics. In this project, we will compare the performance of different methodologies for finding the ground state of the molecule BeH2. We will use circuit cutting and knitting technique, to implement an algorithm which uses classical methods to augment the computation. This will involve an encoding and feedback during, before, and after training.  We will use Qiskit Runtime for error mitigation. We will tackle the barren plateau problems through AdaptVQE.


we describe the implementation of different methodologies to find the ground state of the molecule BeH2, each with their own merits and drawbacks. The methods used consider only single and double excitations. Some of the methodologies that we implement greatly simplify the model while sacrificing chemical accuracy while others use error mitigation more efficiently through qiskit runtime which works well with hybrid algorithms such as VQE.

We are trying to find the ground state of BeH2, so it is worth knowing more on its physical chemistry. Beryllium has chemical formula 1s2 2s2 and the two hydrogens 1s1 in electron configuration notation. When the molecule BeH2 is formed, the s orbitals from the two hydrogens hybridize with the p orbitals from beryllium to form two sp molecular orbital bonds that want to be as far away from each other as possible due to electron repulsion and this results in a linear molecule. We use the sto3g basis to approximate slater type orbitals.

The first method is based on a crude approximation, restricting the Hilbert space to an active space defined by unbonded electrons within the BeH2 molecule.
