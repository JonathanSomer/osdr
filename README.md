![](https://img.shields.io/badge/python-3.10+-blue.svg)
[![codecov](https://codecov.io/gh/JonathanSomer/osdr/branch/v5/graph/badge.svg?token=ybWCucx2Ha)](https://codecov.io/gh/JonathanSomer/osdr)
![Test](https://github.com/JonathanSomer/osdr/actions/workflows/test.yml/badge.svg)
![Format](https://github.com/JonathanSomer/osdr/actions/workflows/format.yml/badge.svg)
![Lint](https://github.com/JonathanSomer/osdr/actions/workflows/lint.yml/badge.svg)
![Typecheck](https://github.com/JonathanSomer/osdr/actions/workflows/typecheck.yml/badge.svg)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square)](https://opensource.org/licenses/Apache-2.0)


# Getting Started

## Requirements

Make sure you have Python 3.10 or higher installed.

```bash
python --version
```

[Optional] setup and activate a new virtualenv:

```bash
python -m venv .venv
source .venv/bin/activate
```

## Installation

### Option 1: Install the package from Github (recommended)

```bash
pip install git+https://github.com/JonathanSomer/osdr.git
```

### Option 2: Install the package locally for development

The following commands will clone the repo and install the `tdm` package locally:

```bash
git clone git@github.com:JonathanSomer/osdr.git
pip install -e ./osdr
```

> **Note:** The `-e` flag is used to install the package in editable mode, which allows you to make changes to the code and have them reflected in the installed package without needing to reinstall.

> **Tip:** You can clone the repo into any directory, just make sure to modify the path `./osdr` provided to the `pip install` command.

## Testing the installation

After installation the following command should display the value `1e-06`:

```bash
python -c "from tdm.utils import microns; print(microns(1))"
```


## Next steps

Check out some [examples](https://jonathansomer.github.io/osdr/examples.html), including figures from our paper "Temporal Tissue Dynamics from a Spatial Snapshot" (Somer, Mannor, Alon, 2025).


# Disclaimer:

This package is released primarily for reproduction of results from the paper by Somer, Mannor, Alon in Nature 2025. We are working on several extensions of this work on a separate development repository and will not be constantly updating this one. 

In general, application of our approach requires some expertise in biology, dynamical systems, statistics and programming. From our experience, debugging a single peculiar phase-portrait could span all of these domains - requiring an understanding of how a biological phenomena could skew a statistical estimate that is then expressed in the phase-portrait. 

Remember: the package will plot a phase-portrait even if underlying assumptions aren’t satisfied. It is your responsibility as a scientist to evaluate a result's validity through the various means we described in the paper, and very likely other means we cannot yet imagine for some applications. Examples include: patient-level or spatial confounders, challenges estimating the death rate, insufficient sample size and analyzing dynamics in state-space regions with minimal data.

Please read our paper carefully, and if you are working on a particularly interesting application - feel free to reach out and we could potentially collaborate.

jonathan.somer@gmail.com
