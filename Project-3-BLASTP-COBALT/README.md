# Project 3 — Protein Sequence Similarity Analysis Using BLASTP and COBALT

## Overview

This project introduces protein sequence analysis using the **NCBI Protein BLAST (BLASTP)** and **COBALT** tools.

The sequence analysed in this project is a 129-residue hen egg-white lysozyme sequence. The main goal was to identify similar known protein sequences and examine sequence conservation among related proteins.

## Biological Question

Which known protein sequences are most similar to the lysozyme sequence being studied?

## Tools Used

- NCBI Protein BLAST (BLASTP)
- NCBI COBALT
- Protein sequence databases

## Query Sequence

The query sequence represented the 129-residue hen egg-white lysozyme sequence used in the earlier structural projects.

The sequence begins with:

`KVFGRCELAA`

This allowed the sequence analysis to be connected with the structural analysis performed in Projects 1 and 2.

## Method

1. Submitted the protein sequence to NCBI Protein BLAST.
2. Examined the ranked protein matches.
3. Compared sequence identity, positives, gaps, E-value and bit score.
4. Identified closely related avian lysozyme sequences.
5. Opened COBALT to begin a multiple sequence alignment analysis.

## Main BLASTP Results

| Hit | Identity | Positives | Gaps | E-value | Score |
|---|---:|---:|---:|---:|---:|
| 1LSG_A — HEN EGG WHITE LYSOZYME [Gallus gallus] | 129/129 (100%) | 129/129 (100%) | 0/129 | 4e-89 | 266 bits |
| XP_015711651.2 — lysozyme C [Coturnix japonica] | 123/129 (95%) | 126/129 (97%) | 0/129 | 2e-84 | 254 bits |
| ACL81751.1 — lysozyme [Bambusicola thoracicus] | 123/129 (95%) | 124/129 (96%) | 0/129 | 2e-84 | 254 bits |

## Interpretation of the Top Hit

The strongest visible BLASTP result was:

**1LSG_A — HEN EGG WHITE LYSOZYME [Gallus gallus]**

The alignment showed:

- 129/129 identical residues
- 100% identity
- 100% positives
- No gaps
- E-value of 4e-89

This provides strong sequence-level evidence that the query corresponds to hen egg-white lysozyme.

## Related Avian Sequences

The next strong matches included lysozyme sequences from:

- *Coturnix japonica*
- *Bambusicola thoracicus*

Both showed approximately **95% sequence identity** with the 129-residue query.

This demonstrates strong sequence conservation among related avian lysozymes.

## Understanding the BLAST Results

### Identity

Identity refers to amino acids that are exactly the same at corresponding positions in an alignment.

### Positives

Positives include identical amino acids as well as substitutions that are considered chemically similar.

### Gaps

Gaps represent inserted or deleted positions introduced during an alignment.

### E-value

The E-value estimates how many matches of similar quality could be expected by chance in the searched database.

A smaller E-value indicates stronger statistical significance.

### Bit Score

The bit score summarizes the strength of the sequence alignment. Higher scores generally indicate stronger matches.

## COBALT

COBALT was opened as a multiple sequence alignment step.

The returned sequence set contained the query and multiple related lysozyme sequences. However, the recorded COBALT output displayed:

**Graphical Overview: Not available**

Therefore, this project does not claim to have completed a detailed COBALT alignment interpretation.

A full conservation analysis will be performed in a later project.

## Biological Interpretation

The BLASTP results strongly support the identity of the query as hen egg-white lysozyme.

The exact 129-residue match to the reported *Gallus gallus* lysozyme sequence provides sequence-level confirmation, while the highly similar avian sequences demonstrate conservation across related species.

## What I Learned

This project helped me understand that BLAST results contain much more information than simply a protein name.

I learned how to interpret:

- Sequence identity
- Positives
- Gaps
- E-values
- Bit scores
- Ranked sequence matches

I also learned to distinguish between a computational step that was successfully performed and an analysis whose output was not sufficiently available for interpretation.

## Limitations

This project did not include:

- A completed detailed multiple sequence alignment analysis
- Phylogenetic tree construction
- Domain analysis
- Mapping sequence conservation onto the 3D structure

These will provide natural directions for future projects.

## Next Step

The next stage is to examine multiple protein sequences together, identify conserved and variable positions, and investigate evolutionary relationships among the sequences.

## Report

[Download the Project 3 Report](Project_3_BLASTP_COBALT_Clean_Figures.pdf)

## Sources

- NCBI BLAST
- NCBI COBALT
- RCSB Protein Data Bank
