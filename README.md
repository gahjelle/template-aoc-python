# Advent of Code Python Template for Copier

This template creates scaffolding for one day of [Advent of Code](https://adventofcode.com/). It includes tests and can download your personal input data if you have [`advent-of-code-data`](https://pypi.org/project/advent-of-code-data/) installed.

## Quick Start

The first time you use this template you should make sure that you have [Copier](https://copier.readthedocs.io/) installed and optionally `advent-of-code-data` as well. You can install these with pipx and pip:

```console
$ pipx install copier
$ python -m pip install advent-of-code-data
```

Once you have Copier on your system, you can create Advent of Code solution templates as follows:

```console
$ copier gh:gahjelle/template-aoc-python advent_of_code/
```

This will ask you about which **year** and **day** you want to template. You can also provide a puzzle name which will be used as part of the directory name and the comments within your files.

The files are copied into a subdirectory of the `advent_of_code/` directory on your computer. You can change `advent_of_code/` to any other name you want.


## Scripting

You can also use Copier as part of a script. The [documentation](https://copier.readthedocs.io/en/stable/api/) shows how to call Copier as part of a Python script.

On the command line, you can use `-d` to provide answers to questions instead of answering them interactively. On Bash (and possibly other shells), the following will set up all directories for the 2021 event inside of your `aoc/` directory:

```console
$ for day in `seq 25`; do
>     copier gh:gahjelle/template-aoc-python -d year=2021 -d day=$day -d puzzle_name="" aoc/
> done
```

After running this, you'll have 25 subdirectories within `aoc/2021/` with templates for solving each day of Advent of Code with Python.


## Examples

See https://github.com/gahjelle/advent_of_code/tree/main/python for examples using the template.
