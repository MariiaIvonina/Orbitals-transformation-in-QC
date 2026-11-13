# IAO/IBO Analysis for Nucleic Acid Systems

This repository accompanies the chapter:

"Automated Comparative Chemical Bond Analysis Using Intrinsic Atomic and Bond Orbitals with PySCF"

Methods in Molecular Biology (Springer Nature).

The notebook demonstrates how to compute:

- IAOs
- IBOs
- Mayer bond indices in IAO basis
- IBO center classification

using PySCF and visualizes the resulting orbitals.

## Running the notebook

To setup conda environment with required packages, you can run in terminal
```
conda env create -f environment.yml
conda activate pyscf-env
jupyter lab pyscf_orbital_analysis.ipynb
```

## Repository structure

```text
.
├── pyscf_orbital_analysis.ipynb  # Main analysis notebook
├── environment.yml               # Conda environment specification
├── examples/                     # Input molecular geometries in XYZ format
├── IBO_cubes/                    # Generated IBO cube files, grouped by molecule
├── mayer_bond_indices.csv        # Generated Mayer bond indices
├── ibo_classification.csv        # Generated IBO classifications
├── README.md
└── LICENSE
```

Running the notebook regenerates the CSV output files and may overwrite
cube files having the same names in `IBO_cubes/`.

## License

Copyright 2026 Mariia Ivonina

The original code in this repository is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE).

This project uses the PySCF API. PySCF is developed by the PySCF Developers and is distributed under the Apache License 2.0. PySCF source code is not included in this repository.