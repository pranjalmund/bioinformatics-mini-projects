# Project 5 — Multiple Sequence Alignment & Conservation Analysis of Avian Lysozyme

## Overview

This project uses multiple sequence alignment (MSA) to compare lysozyme protein sequences from different bird species.

The aim was to identify conserved regions and understand how sequence conservation can be related to the biological function of lysozyme.

## Research Question

Which regions of avian lysozyme are conserved across different bird species, and what might this conservation tell us about protein function?

## Dataset

Three lysozyme protein sequences were used:

| Accession | Species | Protein |
|---|---|---|
| NP_990612.2 | *Gallus gallus* | Lysozyme C |
| XP_015711651.2 | *Coturnix japonica* | Lysozyme |
| ACL81751.1 | *Bambusicola thoracicus* | Lysozyme |

The sequences were selected because they represent closely related avian lysozyme proteins.

## Method

The sequences were examined using sequence-analysis resources including NCBI and COBALT.

The workflow was:

1. Identify lysozyme protein sequences.
2. Collect the protein accession numbers.
3. Compare the sequences using multiple sequence alignment.
4. Examine conserved and variable regions.
5. Relate conserved regions to the known biological role of lysozyme.

## Multiple Sequence Alignment

Multiple sequence alignment places homologous amino acids into corresponding positions so that conserved and variable regions can be examined across several sequences.

For closely related lysozyme proteins, a large proportion of the sequence is expected to remain conserved because the protein performs an important biological function.

The alignment analysis showed strong sequence similarity among the selected avian lysozyme proteins.

## Conservation Analysis

Several regions of the sequences were highly conserved across the selected species.

This is biologically meaningful because lysozyme has an important antimicrobial function. Conserved residues and regions are more likely to contribute to maintaining the protein's structure or activity.

At the same time, some positions showed sequence variation between species.

Such variable positions can arise through evolutionary divergence while still allowing the protein to retain its overall function.

## Biological Interpretation

Lysozyme is an antimicrobial enzyme that contributes to innate immune defence.

Its function depends on maintaining an appropriate three-dimensional structure and catalytic properties. Therefore, strong conservation across related species suggests that important structural and functional constraints act on the protein sequence.

The presence of both conserved and variable positions illustrates an important principle of molecular evolution:

**Functionally important regions tend to be conserved, while other regions can tolerate greater sequence variation.**

## Key Findings

1. The selected avian lysozyme sequences showed high overall similarity.
2. Multiple sequence alignment revealed substantial conservation.
3. Some positions varied between species.
4. Conserved regions are likely to be important for maintaining lysozyme structure and function.
5. Sequence variation demonstrates evolutionary divergence among the species.

## Limitations

This project was designed as a beginner-level sequence-analysis exercise.

Exact column-by-column conservation percentages were not calculated because the available online alignment interface did not consistently expose all requested sequence records in a reproducible format.

Therefore, the conclusions are based primarily on sequence similarity and qualitative conservation patterns rather than a formal statistical conservation score.

## What I Learned

This project helped me understand:

- what multiple sequence alignment is
- why homologous proteins are aligned
- the difference between conserved and variable positions
- how sequence conservation can provide clues about protein function
- how evolutionary changes can occur without necessarily destroying protein function
- how bioinformatics tools can be used to study biological questions

## Tools Used

- NCBI Protein
- NCBI BLASTP
- NCBI COBALT
- RCSB Protein Data Bank
- Multiple sequence alignment concepts

## References

- NCBI Protein and Gene databases
- NCBI COBALT Multiple Sequence Alignment Tool
- RCSB Protein Data Bank
- Project 3 — BLASTP & COBALT Analysis

## Conclusion

The comparison of avian lysozyme sequences demonstrated strong conservation together with limited sequence variation.

This provides a simple example of how multiple sequence alignment can connect molecular sequence data with biological function and evolutionary conservation.
