# numPy-operations

A small collection of examples, notebooks and scripts demonstrating common and useful NumPy operations, patterns, and idiomatic usage for data science and numerical computing.

This repository is intended as a learning resource and quick reference for:

- Array creation and indexing
- Broadcasting and vectorized operations
- Linear algebra and reductions
- Random numbers, sampling and simulations
- Performance tips and comparisons to plain Python loops

## Requirements

- Python 3.8+
- pip

Recommended (not required) packages:

- numpy
- pandas
- matplotlib
- jupyter

## Installation

1. Create a virtual environment (recommended):

```powershell
# create env folder named `venv` and activate it (PowerShell)
python -m venv venv
.\venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
pip install --upgrade pip
pip install numpy pandas matplotlib jupyter
```

(Optional) If a `requirements.txt` appears in this repo in the future, install with:

```powershell
pip install -r requirements.txt
```

## Usage

Open the notebooks or run example scripts to try the exercises and demonstrations.

Start Jupyter Notebook or Jupyter Lab:

```powershell
jupyter notebook
# or
jupyter lab
```

Examples (Python REPL or a .py file):

```python
import numpy as np

# create arrays
a = np.array([1, 2, 3])
B = np.arange(6).reshape(2, 3)

# broadcasting
x = a + B  # adds a to each row of B

# reductions
mean = np.mean(B, axis=1)

print(B)
print(x)
print(mean)
```

## Notebooks and Scripts

This repository focuses on short, self-contained examples. Look for `.ipynb` files and small scripts in the project root or folders. If you open a notebook, run the cells sequentially.

## Contributing

Contributions are welcome. If you'd like to add a new example, notebook, or fix an existing one:

- Open an issue describing the addition or bug
- Send a pull request with a clear description and minimal reproduction (for bugs)
- Keep changes small and focused

Guidelines:

- Follow the existing code style (simple, educational examples)
- Prefer small notebooks or single-purpose scripts
- Add tests/examples where appropriate

## Running tests

There are no automated tests included by default. If you add tests, use a simple runner like `pytest` and add instructions here.

## License

This repository is released under the MIT License. If you need a different license, update this section accordingly.

---

If you'd like, I can:
- add a `requirements.txt` file with pinned versions,
- generate a short example notebook in `notebooks/` with step-by-step numpy exercises, or
- add a pre-commit/CI check to run a linter or tests.

Tell me which follow-up you'd prefer and I'll implement it.