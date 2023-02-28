
ADAPT VQE (Pennylane): In the Single-Double-gates file, we tried using ADAPT VQE for 4 electron and 6 orbitals with noiseless simulator. Note that this corresponds to freezing/removing the core orbital of 1s for Be atom. We use UCCSD ansatz with single and double excitations. For different such excitations, we look at the gradient and remove the excitations for which the gradient is 0. After using only non-zero excitations, we use it as the ansatz to get the GS Energy value as -14.8244 Ha

Even though this value is the lowest among any other (electron,orbital) combination, it's not good enough as we got better results using another method described above.


Implementation of paper: Doubling the Size of Quantum Simulators by Entanglement Forging by Andrew Eddins
We implement the circuit of this paper for BeH2 using entanglement forging. We get a convergence but it converges to a suboptimal value. This suggests that the Ansatz provided in the paper is not based on the state generated, but rather the overall molecule through classical computation. The idea is to do a Schmidt decomposition of circuit into two parts with an interacting term. After 2 X gates, we get the same \phi state as mentioned in the paper. Perhaps, either one needs more hop gates or the effective computation bottleneck is determined by the classical comptutation instead. 
