# 3D Pocket-Based Drug Discovery

Structure-based drug design driven by 3D protein binding pockets: detect and characterise pockets on target structures, then generate, dock and rank ligands against them.

> Status: early development.

## Repository layout

```
.
├── src/pocket3d/      # Python package (pocket detection, featurisation, scoring)
├── tests/             # pytest test suite
├── notebooks/         # Exploratory Jupyter notebooks
├── scripts/           # Command-line entry points and pipelines
├── configs/           # YAML run configurations
├── data/
│   ├── raw/           # Input structures (PDB/mmCIF, SDF) — not tracked by git
│   └── processed/     # Derived pockets, features — not tracked by git
└── results/           # Run outputs — not tracked by git
```

## Installation

```bash
git clone https://github.com/<your-username>/3d-pocket-drug-discovery.git
cd 3d-pocket-drug-discovery

conda env create -f environment.yml
conda activate pocket3d
pip install -e ".[dev]"
```

## Usage

```python
import pocket3d
print(pocket3d.__version__)
```

## Testing

```bash
pytest
```

## Citation

If you use this work, please cite it using the metadata in [CITATION.cff](CITATION.cff).

## License

Released under the MIT License, see [LICENSE](LICENSE).

## Contact

Shaurya, shaurya@nii.ac.in
