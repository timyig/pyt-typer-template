# pyt-typer-template

Template for a Python CLI application using [Typer](https://typer.tiangolo.com/)  
[Typer GitHub repository](https://github.com/tiangolo/typer)

## Roadmap

- [x] Add requirements with conda
- [x] Add logging
- [x] Add linting
- [ ] Add formatting
- [ ] Add type checking
- [ ] Add three CLI commands with typer
- [ ] Add tests
- [ ] Add code coverage
- [ ] Add code formatting
- [ ] Add pre-commit hooks
- [ ] Add CI/CD for Ubuntu and Windows
- [ ] Convert to a cookiecutter template

## Requirements

### CI/CD

- Run test on Ubuntu and Windows
- pre-commit hooks
  - black
  - flake8
  - mypy
  - pytest
  - coverage


### Python
- dependencies with [conda](https://docs.conda.io/en/latest/)
- Logging with [loguru](https://loguru.readthedocs.io/en/stable/)
- linting with [flake8](https://flake8.pycqa.org/en/latest/)
- testing with [pytest](https://docs.pytest.org/en/stable/)
- code coverage with [coverage](https://coverage.readthedocs.io/en/coverage-5.5/)
- code formatting with [black](https://black.readthedocs.io/en/stable/)
- type checking with [mypy](https://mypy.readthedocs.io/en/stable/)

### CLI
- [Typer](https://typer.tiangolo.com/)

- Printing with [rich](https://rich.readthedocs.io/en/latest/)
- CLI template functions
  - init
    - load config
    - create logger
  - run
    - create list of files to process
    - process files
    - print results with progress bar
  - clean
    - remove files


### Devenv

Designed to work with Github Codespaces

## Usage

### Install dependencies

### Running in Codespace

```bash
  conda activate $CONDA_ENV_NAME
```

### Not in Codespace

Install conda if not already installed or not running in a Codespace

```bash
  # https://docs.conda.io/projects/miniconda/en/latest/

  mkdir -p ~/miniconda3
  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
  bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
  rm -rf ~/miniconda3/miniconda.sh
```

Create conda environment

```bash
  conda env create --file environment.yml
  conda activate typer_template
```

Update conda environment with new dependencies

```bash
  conda env update
```