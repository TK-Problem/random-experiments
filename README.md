# random-experiments

A collection of small ML/statistics experiments in Jupyter notebooks. All experimetns can be run via google colab.

## Notebooks

| # | Notebook | Description |
|---|----------|-------------|
| 001 | `001_bayesian_linear_model.ipynb` | Bayesian linear regression on SPY daily returns using PyMC |

---

## Local setup with uv

[uv](https://docs.astral.sh/uv/) must be installed. If it isn't:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Clone and enter the repo

```bash
git clone https://github.com/TK-Problem/random-experiments.git
cd random-experiments
```

Create the virtual environment and install dependencies

```bash
uv sync
```

`uv sync` reads `pyproject.toml`, creates a `.venv` with Python 3.13 (pinned in `.python-version`), and installs all dependencies from `uv.lock`.

Register the environment as a Jupyter kernel

```bash
uv run python -m ipykernel install --user --name random-experiments --display-name "random-experiments"
```
---