# Crosswizard

Crosswizard fills in a crossword. You give it a grid with some squares already filled and a word list, and it works out a set of intersecting words that complete the grid. It is a small project I built to get the constraint-solving right: the interesting part is the backtracking search and the pruning that keeps it fast.

## How it works

The solver places words one slot at a time and backtracks whenever a placement leaves a slot with no valid word left. The speedups come from checking the board state as it goes, so it abandons a branch the moment the letters already on the board rule out every remaining candidate, instead of filling the whole grid and discovering the conflict at the end. Candidate words are looked up from a bundled list of about twenty thousand words.

## Running it

The solver lives in `Xwords2.py` and runs from the command line. The `20k.txt` word list ships with the repo, so you can try it right away. There is a worked example in the code comments showing the grid input format, which is compact and takes a minute to read before your first run.

```bash
python Xwords2.py
```

## Notes and limitations

- The grid input format is terse. It is documented in the file, but it is meant for driving the solver rather than for hand-authoring large puzzles.
- Everything lives in a single file. The point of the project was the algorithm, not the packaging.
- There is no GUI. Output is printed to the terminal.
