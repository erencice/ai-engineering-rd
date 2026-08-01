# Applied Theorem Path

An interactive, code-driven curriculum for the mathematical foundations of machine learning. Concepts are introduced with rigorous definitions and proofs, then made concrete through runnable Jupyter notebooks with finite-set simulations, counterexamples, and visualizations tied to ML.

## Structure

```
curriculum/
└── foundations/            # Foundational math for ML theory
    ├── 00-basic-logic-and-proof-techniques.ipynb
    ├── 01-Cantor_Theorem_IEEE_EN.pdf
    └── 01-sets-functions-and-relations.ipynb
```

## Foundations

### 00 — Basic Logic and Proof Techniques

Companion notebook covering the logical toolkit used throughout math and ML theory:

- Propositions, implications, and truth tables
- Universal/existential quantifiers and their negations
- Proof techniques: direct, contrapositive, contradiction, induction, construction, cases, counterexamples
- Common confusions (contrapositive vs. converse, vacuous truth)
- Quick drills and exercises with runnable solutions (e.g., PAC-style bound templates)

### 01 — Sets, Functions, and Relations

Interactive companion to the [Sets, Functions, and Relations](curriculum/foundations/01-Cantor_Theorem_IEEE_EN.pdf) source:

- Sets and operations; power sets and cardinality
- Functions, images/preimages, composition, and inverses
- Equivalence relations and quotient sets
- Cantor's Theorem (diagonalization) and Schröder–Bernstein Theorem with finite-set simulations
- ML connections: equivalence classes of classifiers, VC dimension of threshold/linear classifiers, Cartesian products in feature spaces
- Relations and partial orders
- Exercises with verified solutions

## Usage

Open a notebook and run it interactively:

```bash
jupyter notebook curriculum/foundations/
```

or without a browser:

```bash
jupyter nbconvert --to notebook --execute curriculum/foundations/00-basic-logic-and-proof-techniques.ipynb
```

Dependencies: Python 3 with `numpy` and `matplotlib` (used in the visualizations and simulations).