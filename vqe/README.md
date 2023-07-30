# vqeH2


The realm of quantum physics and computing stands as a beacon of intrigue and promise in our modern era. It holds vast potential, from advancing communication networks for speed and security to unraveling the complexities of protein folding. Within this domain, the Variational Quantum Eigensolver (VQE) emerges as a noteworthy algorithm, blending classical and quantum approaches to tackle optimization challenges.


One compelling application for this algorithm is its ability to compute the energy of molecular Hydrogen (H2), a prominent alternative to methane. Yet, this is merely a starting point. The versatility of VQE extends to comprehending a spectrum of molecules pivotal across the energy landscape, spanning solar cell materials, battery constituents, carbon capture mechanisms, hydrogen storage solutions, and virtually any chemical scenario. This broad utility promises efficiency gains, cost savings, and resource optimization. Here, we witness VQE in action as it elucidates the electronic structure of H2 at different Angstrom distances between its atoms.

### Instructions
1. Convert a molecule into a ‘QMolecule’ with varying distances between the H atoms.
2. Define a tunable circuit using ‘EfficientSU2’, mapping atoms to qubits where each qubit represents the state of an atom or particle.
   We also use the classical optimizer algorithm ‘COBYLA’ that employs linear approximations to objective and constraint functions.
3. Find the total energy through both VQE and an exact solver (to verify results) in addition to calculating percent error.

<br>

Tunable Circuit

<img width="433" alt="Screenshot 2023-08-10 at 7 26 22 AM" src="https://github.com/jaszmine/vqeH2/assets/52623824/a736afbf-6196-4cb5-8185-ecfef3ef9b97">

<br>
<br>

Total energies using vqe and exact solver w/percent error

<img width="600" alt="Screenshot 2023-08-10 at 7 28 50 AM" src="https://github.com/jaszmine/vqeH2/assets/52623824/6319144e-b5a8-47cc-91ba-aef098d59e29">

<br>
<br>

<img width="600" alt="Screenshot 2023-08-10 at 2 38 29 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/cb09015b-2b02-42d7-a893-585aa230e010">

<br>
<br>

<img width="600" alt="Screenshot 2023-08-10 at 2 38 41 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/fc86382c-dff3-40c5-9012-97a85231bad3">


<br>
<br>
<br>

Visualization of Exact Solver vs. VQE methods 

<img width="576" alt="Screenshot 2023-08-10 at 2 28 32 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/96c801f2-bc34-4cc2-b277-8e16f5f0d30a">

<br>
<br>

Analysis demonstrates we can see the relative accuracy and time it takes for VQE to reach the optimal solution/energy compared to the exact solver. Now imagine using this method with much more complicated molecules with far more atoms than H2.

While VQE has shown immense promise, there are some limitations we have to consider such as available quantum resources, circuit complexity, error mitigation, and scalability. However, as we begin to improve both quality and quantity regarding quantum hardware, the prospects of VQE continue to grow. 

