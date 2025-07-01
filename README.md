Cu-Sn Machine Learning Interatomic Potential
This repository contains a machine learning interatomic potential (MLIP) model for the Cu-Sn alloy system, developed using the Deep Potential Generator (DP-GEN) and DeepMD-kit frameworks. The trained model is provided as frozen_model.pb.
Using this DP model, we performed molecular dynamics (MD) simulations to compute the energy–volume (E–V) curve, elastic moduli, and phonon spectra of Cu-Sn compounds. The simulation results show excellent agreement with density functional theory (DFT) calculations, demonstrating that the developed model achieves DFT-level accuracy while maintaining significantly higher computational efficiency.
Software Used
DP-GEN: Automated active learning workflow for training interatomic potentials
DeepMD-kit: Neural network potential training package
LAMMPS: Molecular dynamics engine for simulation
Repository Structure
├── result/                 # MD results: energy–volume curves, phonon spectra
├── Dataset/
│   ├── init_data/          # Initial dataset used to bootstrap DP-GEN
│   └── training_data/      # New data added during iterative training
├── frozen_model.pb         # Final trained Deep Potential model
└── report/                 # Experimental report and summary
