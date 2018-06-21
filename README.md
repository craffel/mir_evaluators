# `mir_eval` evaluators

This repository contains scripts which can be run from the command line and utilize `mir_eval` to compute metrics according to reference and estimated annotations you provide.
To use the evaluators, you must first install `mir_eval` and its dependencies (see [here](https://craffel.github.io/mir_eval/#installing-mir-eval)).

## Usage

By way of example, we'll cover the usage of the beat detection evaluator ``beat_eval``.
To use an evaluator for a different task, simply replace ``beat_eval`` in the following with the name of the evaluator for the task you're interested in.
To get usage help, simply run

`./beat_eval.py --help`

As an example, to evaluate generated beat times stored in the file `estimated_beats.txt` against ground-truth beats stored in the file `reference_beats.txt` and store the resulting scores in `results.json`, simply run

`./beat_eval.py -o results.json reference_beats.txt estimated_beats.txt`

The file `results.json` will now contain the achieved scores in machine-parsable, human-readable json format.  Nice!
