# Project 2 — Comparative Structural Analysis of 1FDL and 1AKI

## Overview

This project compares the structure of hen egg-white lysozyme in two different structural contexts:

- **1AKI** — lysozyme in its free state
- **1FDL** — lysozyme bound to the Fab D1.3 antibody

The purpose of this project is to examine whether the overall three-dimensional structure of lysozyme remains similar when it is present alone versus when it is part of an antibody–antigen complex.

## Biological Question

Does hen egg-white lysozyme maintain a similar overall three-dimensional structure in its free state and antibody-bound state?

## Structures Compared

| Feature | 1AKI | 1FDL |
|---|---|---|
| Protein | Hen egg-white lysozyme | Hen egg-white lysozyme |
| State | Free | Antibody-bound |
| Lysozyme chain | Chain A | Chain C (auth Y) |
| Length | 129 residues | 129 residues |
| Experimental method | X-ray diffraction | X-ray diffraction |
| Resolution | 1.50 Å | 2.50 Å |

## Method

The two structures were explored using the RCSB Protein Data Bank and Mol* molecular visualization.

The lysozyme chain from each structure was examined and the overall three-dimensional shapes were visually compared.

A quantitative structural comparison using pairwise structural alignment was also performed to assess the similarity more objectively.

## Observations

The overall fold of lysozyme appears broadly similar in the two structures.

The free lysozyme structure in 1AKI and the antibody-bound lysozyme in 1FDL both show the characteristic compact globular structure of lysozyme.

The difference in structural context is that lysozyme is present alone in 1AKI, whereas it forms an antibody–antigen complex in 1FDL.

## Quantitative Comparison

A pairwise structural alignment of the lysozyme chains was performed using:

- **1AKI, Chain A**
- **1FDL, Chain C (auth Y)**

The alignment showed:

- **RMSD:** 0.37 Å
- **TM-score:** 0.99
- **Sequence identity:** 100%
- **Aligned residues:** 129 / 129

These results indicate an extremely high structural similarity between the two lysozyme structures.

## Interpretation

The very low RMSD and high TM-score indicate that the overall three-dimensional fold of lysozyme is highly conserved between the free and antibody-bound structures.

This suggests that antibody binding does not produce a major change in the overall fold of lysozyme.

However, this does not mean that antibody binding has absolutely no structural effect. Local conformational changes may still occur, particularly near the antibody–antigen interface.

## What I Learned

Through this project, I learned how structural context can be compared using experimentally determined protein structures.

I also learned the difference between qualitative visual comparison and quantitative structural comparison using measures such as RMSD and TM-score.

## Limitations

This project focuses mainly on overall structural similarity.

A more detailed analysis could investigate residue-level structural differences, interface contacts, hydrogen bonds, and local conformational changes around the antibody-binding region.

## Tools Used

- RCSB Protein Data Bank
- Mol*
- RCSB Pairwise Structure Alignment
- TM-align

## Conclusion

Hen egg-white lysozyme shows a highly similar overall three-dimensional structure in the free 1AKI structure and the antibody-bound 1FDL structure.

The quantitative alignment supports the visual observation, with an RMSD of 0.37 Å and a TM-score of 0.99 across all 129 aligned residues.

This project demonstrates how structural bioinformatics can be used to compare protein conformations across different biological contexts.
