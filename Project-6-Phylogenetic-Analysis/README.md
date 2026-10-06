# Project 6 — Phylogenetic Analysis of Avian Lysozyme

## Overview

This project explores evolutionary relationships among lysozyme proteins from different bird species using sequence similarity.

The purpose was to understand how protein sequence comparison can be used to visualise evolutionary relationships between closely related organisms.

## Research Question

How can sequence similarity be used to visualise evolutionary relationships among closely related avian lysozyme proteins?

## Dataset

Three avian lysozyme proteins were considered:

| Accession | Species | Protein |
|---|---|---|
| NP_990612.2 | *Gallus gallus* | Lysozyme C |
| XP_015711651.2 | *Coturnix japonica* | Lysozyme |
| ACL81751.1 | *Bambusicola thoracicus* | Lysozyme |

These proteins were selected as a small educational dataset for exploring sequence similarity and evolutionary relationships.

## Method

The analysis was based on sequence similarity obtained during the previous BLASTP analysis.

The workflow was:

1. Identify homologous avian lysozyme sequences.
2. Compare their protein sequences using BLASTP.
3. Examine pairwise sequence similarity.
4. Use the similarity relationships to visualise a simple phylogenetic relationship.
5. Interpret the results in an evolutionary context.

## Pairwise Similarity

The BLASTP analysis from Project 3 showed high similarity among the selected sequences.

| Comparison | Approximate sequence identity |
|---|---:|
| *Gallus gallus* vs *Coturnix japonica* | 95% |
| *Gallus gallus* vs *Bambusicola thoracicus* | 95% |

The high sequence identity indicates that these proteins are closely related homologs.

## Phylogenetic Interpretation

The similarity relationships were visualised as a simple phylogenetic-style tree.

The closely related sequences cluster together because they share a high degree of sequence similarity.

The tree provides an intuitive way to represent the relationships suggested by the sequence comparisons.

## Important Note About the Tree

This project uses a **small educational dataset** and the tree is intended primarily as a visualisation of sequence relationships.

It should not be interpreted as a publication-quality evolutionary phylogeny.

A rigorous phylogenetic analysis would require:

- a larger set of homologous sequences
- a reproducible multiple sequence alignment
- an explicitly selected tree-building method such as Neighbor Joining or Maximum Likelihood
- appropriate evolutionary models
- bootstrap or other branch-support analysis
- careful selection of orthologous sequences

## Biological Interpretation

The strong sequence similarity among the avian lysozyme proteins is consistent with conservation of an important antimicrobial protein across related bird species.

The high similarity suggests that evolutionary constraints have maintained much of the lysozyme sequence while allowing some variation between species.

This demonstrates how sequence-based bioinformatics can be used to connect molecular similarity with evolutionary relationships.

## Key Findings

1. The selected avian lysozyme proteins showed high sequence similarity.
2. Chicken, quail and Bambusicola lysozyme sequences were suitable for a small comparative analysis.
3. Pairwise identities were approximately 95% for the comparisons examined.
4. High sequence similarity supports close evolutionary relatedness among these homologous proteins.
5. A phylogenetic-style tree provides a simple visual representation of these relationships.

## Limitations

The dataset contains only three sequences, which is too small for a robust phylogenetic study.

The analysis also does not include bootstrap support or a formally inferred maximum-likelihood tree.

Therefore, the tree should be treated as an educational visualisation rather than definitive evidence of species evolutionary history.

## What I Learned

This project helped me understand:

- the relationship between sequence similarity and evolutionary relatedness
- how homologous proteins can be compared
- how phylogenetic trees represent relationships
- why larger datasets are needed for reliable phylogenetic inference
- why bootstrap support and explicit tree-building methods are important
- the difference between an educational analysis and a publication-quality phylogenetic study

## Tools Used

- NCBI BLASTP
- NCBI Protein
- NCBI COBALT
- RCSB Protein Data Bank
- Basic phylogenetic concepts

## References

- NCBI Protein and BLAST databases
- RCSB Protein Data Bank
- Project 3 — BLASTP & COBALT Analysis
- Project 5 — Multiple Sequence Alignment & Conservation Analysis

## Conclusion

This project demonstrated how protein sequence similarity can be used to explore evolutionary relationships.

Although the dataset was intentionally small, it provided a practical introduction to phylogenetic thinking and showed why sequence-based comparisons are an important part of bioinformatics.
