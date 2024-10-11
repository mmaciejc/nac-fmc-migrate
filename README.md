# INSTRUCTION

## Installation

This project uses [Poetry](https://python-poetry.org/) for dependency management.

You can install the project with the following command:

```bash
poetry install
```

Or with pip:

```bash
pip3 install .
```

## Usage

```cli
Usage: nac-migrate [OPTIONS]

Options:
  -s, --solution [FMC]      Solutions supported [FMC]  [required]
  -f, --from TEXT           YAML file of OLD FMC configuration  [required]
  -t, --to TEXT             YAML file of existing FMC configuration  [required]
  -w, --what TEXT           YAML file with objects to be migrated  [required]
  -v, --verbose             Enable verbose output
  --help                    Show this message and exit.
```

## FMC

If you installed with `poetry install` command:

```sh
poetry run nac-migrate -s FMC --from old_fmc.yaml --to new_fmc.yaml --what to_migrate.yaml -v DEBUG 
```

If you installed the project with pip, you can run the script directly from the command line:

```sh
nac-migrate -s FMC --from old_fmc.yaml --to new_fmc.yaml --what to_migrate.yaml -v DEBUG 
```