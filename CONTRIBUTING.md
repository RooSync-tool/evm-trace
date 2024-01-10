# Development

To get started with working on the codebase, use the following steps prepare your local environment:

```bash
# clone the github repo and navigate into the folder
git clone https://github.com/ApeWorX/evm-trace.git
cd evm-trace

# create and load a virtual environment
python3 -m venv venv
source venv/bin/activate

# install evm-trace into the virtual environment
python setup.py install

# install the developer dependencies (-e is interactive mode)
pip install -e .'[dev]'
```

## Pre-Commit Hooks

We use [`pre-commit`](https://pre-commit.com/) hooks to simplify linting and ensure consistent formatting among contributors.
Use of `pre-commit` is not a requirement, but is highly recommended.

Install `pre-commit` locally from the root folder:

```bash
pip install pre-commit
pre-commit install
```

Committing will now automatically run the local hooks and ensure that your commit passes all lint checks.


