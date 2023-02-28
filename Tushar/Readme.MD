Using simple VQE with active electrons gives not so good results with energy -14.8


Using VQE with only significant single and double gates also gives the energy -14.84, not efficient


ADAPT VQE (Pennylane): In the Single-Double-gates file, we tried using ADAPT VQE for 4 electron and 6 orbitals with noiseless simulator. Note that this corresponds to freezing/removing the core orbital of 1s for Be atom. We use UCCSD ansatz with single and double excitations. For different such excitations, we look at the gradient and remove the excitations for which the gradient is 0. After using only non-zero excitations, we use it as the ansatz to get the GS Energy value as -14.8244 Ha

Even though this value is the lowest among any other (electron,orbital) combination, it's not good enough as we got better results using another method described above.

