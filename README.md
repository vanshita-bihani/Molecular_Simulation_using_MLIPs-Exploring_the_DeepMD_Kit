# Molecular-Simulation-using-MLIPs-Exploring-the-DeepMD-Kit-


Classical force
f
ields, while computationally inexpensive and capable of simulating millions of atoms,
rely on empirical parameterization that often fails to capture complex chemical phe
nomena such as bond breaking, polarization, or specific electronic states. Conversely,
ab initio methods like Density Functional Theory (DFT) offer high fidelity but scale
poorly with system size (O(N3)), effectively limiting simulations to small clusters and
short timescales.
This report addresses this fundamental limitation by exploring the implementation
of Machine Learning Interatomic Potentials (MLIPs), specifically utilizing the Deep
Potential (DP) framework via the DeePMD-kit software package. We present a com
prehensive ”data-to-discovery” pipeline, demonstrating the training, validation, and
deployment of neural network-based potentials trained on high-fidelity quantum data.
As a primary validation case study, we model the thermodynamic and transport
properties of methane (CH4), a system governed by a challenging interplay of stiff
intramolecular covalent bonds and weak intermolecular dispersion forces. The Deep
Potential model is rigorously validated against structural benchmarks, reproducing the
Carbon-Hydrogen bond length derived from the Radial Distribution Function (RDF)
with a peak at approximately 1.1˚ A, in agreement with the experimental value of
1.09˚
A. Furthermore, the model is deployed to simulate bulk liquid methane, success
fully predicting macroscopic transport properties including the self-diffusion coefficient
(D ≈2.3×10−9m2/s) via Mean Square Displacement (MSD) and thermal conductivity
(κ) via the Green-Kubo formalism.
