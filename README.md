# `mir_eval` evaluators

This repository contains some example scripts for running `mir_eval`.
They compute metrics according to reference and estimated annotation files that you provide.
They can be used run from the command line, so that you don't have to write any code.
To use these scripts, you'll need to install `mir_eval` first, for example by running `pip install mir_eval` or installing [from source](https://github.com/craffel/mir_eval/).

## Usage

To run an evaluator script `task_eval.py`, simply run

`./task_eval.py ref_file est_file arguments`

For help,

`./task_eval.py --help`
