**README.md:**

```markdown
# Fix-Phonon-Map-File-Generator

This script generates the map file required by fix-phonon from a data file or POSCAR using Pymatgen. It analyzes the structure file, identifies the primitive cell, and maps the supercell to its primitive components.

## Requirements

- Python 3
- Pymatgen

## Installation

To install Pymatgen, you can use pip:

```sh
pip install pymatgen
```

## Usage

To generate a map file from a POSCAR or a LAMMPS data file, use the following command:

```sh
python map.in_generator_for_fix_phonon_command.py<structure_file> -s <style> -o <output_file> -p <symprec> -a <angtol>
```

### Examples:

To generate a map file from a POSCAR:

```sh
python map.in_generator_for_fix_phonon_command.py POSCAR -s poscar -o map.in -p 0.01 -a 5
```

To generate a map file from a LAMMPS data file:

```sh
python map.in_generator_for_fix_phonon_command.py data.lammps -s atomic -o map.in -p 0.01 -a 5
```

