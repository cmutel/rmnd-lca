# Fork to support Brightway25

This premise fork is using Brightway25, which introduces a few small backwards-incompatible changes. As such, it currently needs a little bit of love and attention to get going.

## Installation

Create a new virtual env. This can be done in conda or pip; I give instructions for pip:

1. Create a new venv:

    python -m venv <venv directory>/premise

2. Activate the venv, e.g.

    source <venv directory>/premise/bin/activate

3. Install the necessary packages:

    pip install brightway25 pypardiso pip install wurst xarray prettytable "carculator>=1.4.3" "carculator_truck>=0.1.5" pycountry cryptography

4. Download the `premise` fork source code, and then edit `setup.py` to remove the dependency on `brightway2`.

5. Do an editable install of the `premise` fork:

    pip install -e .

## Usage
