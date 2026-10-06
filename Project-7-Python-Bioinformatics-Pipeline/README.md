# Project 7 — Python Bioinformatics Pipeline for Protein FASTA Analysis

## Overview

This project introduces a simple Python-based workflow for analysing protein FASTA sequences.

The aim was to understand how basic bioinformatics tasks can be automated using Python instead of performing every calculation manually.

## Research Question

Can a short Python program automate basic protein-sequence quality checks and summary statistics?

## Objective

The main objectives of this project were to:

- Read protein sequences from a FASTA file
- Parse multiple sequence records
- Calculate sequence lengths
- Count selected amino acids
- Search for simple sequence patterns
- Generate a basic summary of the input sequences

## Workflow

The pipeline follows this general workflow:

**FASTA input → Sequence parsing → Quality checks → Sequence statistics → Summary output**

## Python Implementation

The following Python program was developed as a beginner-level FASTA analysis pipeline:

```python
from pathlib import Path

def read_fasta(path):
    records = []
    name, seq = None, []

    for line in Path(path).read_text().splitlines():
        line = line.strip()

        if not line:
            continue

        if line.startswith(">"):
            if name is not None:
                records.append((name, "".join(seq)))

            name = line[1:]
            seq = []

        else:
            seq.append(line.upper())

    if name is not None:
        records.append((name, "".join(seq)))

    return records


def summarize(name, seq):
    return {
        "id": name,
        "length": len(seq),
        "A": seq.count("A"),
        "G": seq.count("G"),
        "C": seq.count("C"),
        "K": seq.count("K"),
        "R": seq.count("R"),
    }


records = read_fasta("lysozyme.fasta")

results = [
    summarize(name, seq)
    for name, seq in records
]

for row in results:
    print(row)
