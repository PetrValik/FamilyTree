# Family Tree

A pure-Python family-tree model that builds a genealogical tree from raw data and supports validation, queries and pretty-printing.

## About

University assignment (Masaryk University, introductory programming course). Given three dictionaries — names, birth years, and parent→children relations — the program constructs a tree of `Person` nodes and offers a set of operations over it:

- **Build & validate** — assemble a single-rooted tree and check its integrity (unique names among siblings, parents older than children, no cycles).
- **Queries** — find childless members, list a person's ancestors, and identify parents younger/older than a given age at a child's birth.
- **Order of succession** — compute succession ranking over a set of living members (depth-first by birth year).
- **Prune** — remove extinct branches (leaf lines with no living members).
- **Pretty-print** — render the tree with Unicode box-drawing connectors (`├─`, `└─`, `│`), optionally names-only.

Fully type-annotated (`typing`), no external dependencies. Developed without AI tools.

## Tech

Python 3 (standard library only).

## Run

```bash
python3 hw5.py        # runs the built-in assertion test suite
```

To see the tree rendering, uncomment the `draw_example()` call at the bottom of `hw5.py`. The assignment specification is in `hw5.html`.
