# Project 4 — Structural Alignment and RMSD Analysis

## Overview

This project compares the three-dimensional structures of hen egg-white lysozyme in two different structural contexts:

- **1AKI** — free hen egg-white lysozyme
- **1FDL** — antibody-bound hen egg-white lysozyme

The aim was to determine how similar the overall protein structures are and whether antibody binding is associated with major structural changes.

## Research Question

How structurally similar is lysozyme when present as a free protein compared with lysozyme bound to an antibody?

## Structures Compared

| Structure | Protein | Chain | Resolution |
|---|---|---|---|
| 1AKI | Hen egg-white lysozyme | A | 1.50 Å |
| 1FDL | Hen egg-white lysozyme | C (author chain Y) | 2.50 Å |

Both lysozyme chains contain **129 residues**.

## Method

The structures were compared using a protein structure alignment approach.

The analysis focused on:

- RMSD (Root Mean Square Deviation)
- TM-score
- sequence identity
- number of aligned residues
- overall structural similarity

The structures were inspected using RCSB PDB structural visualization and pairwise structure-alignment results.

## Results

The structural alignment produced the following results:

| Parameter | Result |
|---|---:|
| RMSD | 0.37 Å |
| TM-score | 0.99 |
| Sequence identity | 100% |
| Aligned residues | 129 / 129 |
| Length compared | 129 / 129 |

## Interpretation

The very low RMSD of **0.37 Å** indicates that the two lysozyme structures have extremely similar three-dimensional conformations.

The **TM-score of 0.99** further supports the conclusion that the global folds are essentially the same.

All 129 residues could be aligned with 100% sequence identity, which is expected because the comparison involves the same lysozyme protein sequence in two structural contexts.

These results suggest that binding to the antibody does not cause a major rearrangement of the overall lysozyme fold.

However, a highly similar global structure does not mean that every local region is identical. The antibody interface identified in Project 1 includes lysozyme residues approximately **18–27 and 117–125**, so local conformational differences may still occur around these regions.

## Key Findings

1. The free and antibody-bound lysozyme structures are highly similar.
2. All 129 residues were structurally aligned.
3. The RMSD was only 0.37 Å.
4. The TM-score was 0.99.
5. The comparison indicates strong conservation of the overall lysozyme fold.
6. Local changes at antibody-contact regions cannot be ruled out from the global RMSD alone.

## Limitations

This analysis focuses mainly on global structural similarity.

RMSD and TM-score do not by themselves identify which individual residues undergo local conformational changes. A residue-level analysis would be required to investigate subtle structural differences around the antibody-binding interface.

## What I Learned

This project helped me understand how protein structures can be quantitatively compared using structural alignment.

I learned the meaning and interpretation of:

- RMSD
- TM-score
- structural alignment
- sequence identity
- aligned residues
- global versus local structural similarity

It also showed me why a single global similarity measure should be interpreted together with biological context.

## Tools Used

- RCSB Protein Data Bank
- RCSB/Mol* structural visualization
- Protein structure alignment tools
- Basic structural biology concepts

## References

- RCSB Protein Data Bank: 1AKI
- RCSB Protein Data Bank: 1FDL
- RCSB PDB structure-alignment resources
