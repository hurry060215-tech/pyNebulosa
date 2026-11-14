# Installation

## Candidate installation

This independent variant is not published yet. From the release checkout:

```bash
python -m pip install .
```

## With scanpy (recommended)

```bash
python -m pip install ".[scanpy]"
```

## Development install

```bash
git clone --branch release/omicverse-nebulosa https://github.com/hurry060215-tech/pyNebulosa.git
cd pyNebulosa
pip install -e ".[dev]"
```

The intended PyPI distribution is `py-nebulosa-omicverse`, imported as
`ov_nebulosa`. It does not overwrite the original `pynebulosa` module.

## Requirements

- Python >= 3.9
- numpy >= 1.22
- scipy >= 1.9
- matplotlib >= 3.5
- anndata >= 0.8
- scanpy >= 1.9 (optional, for loading example datasets)
