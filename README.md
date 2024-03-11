# Electronic structure calculations of small molecules using VQE

This work was part of my master's thesis. Said work focused on the Variational Quantum Eigensolver (VQE) as an alternative approach to solving the electronic structure problem of light molecules, in particular $H_2$, $HeH$, $LiH$ and $BeH$. The accuracy and efficiency of said algorithm is put to the test after compairing its performance to that of other popular computational chemistry methods such as the Hartree-Fock (HF) self-consistent field (SCF) method and an exact diagonalization of the system's Hamiltonian.

The analysis of this algorithm was performed focusing on four aspects: ansatz, basis set, optimizers and backends. The most popular options available for each input were discussed along with the yielded results. Both the code and output graphs can be found on each subsequent folder:

- `potential curves`: shows how to compute the potential curves of the electronic ground state of the molecule, using VQE, HF and NP. This is the 'skeleton' of the rest of the work.
- `basis`: contains the code used to compare STO-3G with 631-G as the basis set of choice for computing the electronic integrals of the hamiltonian.
- `optimizers`: compares the three most popular classical optimization subroutines SLSQP, SPSA and COBYLA under noiseless simulations and fixing UCCSD as the ansatz.
- `noisy simulations`: tests VQE and different ansatz-optimizers combinations to check which pair works the best under noisy circumstances. Error mitigation techniques are also used to better the results.
- `using real quantum devices`: performs a simulation of the algorithm on a real quantum computer provided by IBM. 



