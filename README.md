# Fix-Phonon-Map-File-Generator
This script generates the map file required by fix-phonon from a data file or POSCAR using Pymatgen. It analyzes the structure file, identifies the primitive cell, and maps the supercell to its primitive components.
# Generate Map File for fix-phonon

## Requirements

- Python 3
- Pymatgen

## Installation

To install Pymatgen, you can use pip:

```sh
pip install pymatgen

## To generate a map file from a POSCAR:
```sh
python generate_map.py POSCAR -s poscar -o map.in -p 0.01 -a 5

## To generate a map file from a LAMMPS data file:
```sh
python generate_map.py data.lammps -s atomic -o map.in -p 0.01 -a 5

