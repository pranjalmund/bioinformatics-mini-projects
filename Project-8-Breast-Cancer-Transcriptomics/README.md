# Project 8 — Transcriptomic Analysis of Chemotherapy Response in Breast Cancer

## Overview

This project explores publicly available RNA-seq data from breast cancer patients who received neoadjuvant chemotherapy.

The main goal was to investigate transcriptomic differences between patients who were sensitive to chemotherapy and those who were resistant to treatment.

The project uses the public GEO dataset **GSE162187** and follows a research-oriented bioinformatics workflow from dataset selection to differential-expression interpretation and candidate biomarker analysis.

## Research Question

Which transcriptomic differences are associated with chemotherapy sensitivity or resistance in breast cancer, and which candidate genes show evidence of prognostic relevance?

## Dataset

| Feature | Description |
|---|---|
| GEO accession | GSE162187 |
| Organism | *Homo sapiens* |
| Experiment | RNA-seq gene-expression profiling |
| Patient profiles | 22 |
| Treatment-sensitive | 9 |
| Treatment-resistant | 13 |
| Reference genome | GRCh38 |
| Repository | NCBI Gene Expression Omnibus |

## Computational Workflow

The overall workflow was:

**Public RNA-seq dataset → Expression quantification → Differential expression → Multiple-testing correction → Functional interpretation → Candidate biomarker analysis → External validation**

The original study used Kallisto for transcript quantification and DESeq2 for differential-expression analysis.

Functional interpretation included Gene Ontology, KEGG, GSEA and protein-association analyses.

## Differential-Expression Analysis

The original analysis reported:

**1,985 differentially expressed genes**

between chemotherapy-sensitive and chemotherapy-resistant patients.

The reported enriched biological themes included:

- Metabolic pathways
- Pathways in cancer
- Cytokine–cytokine receptor interactions
- Neuroactive ligand–receptor interactions

These findings suggest that chemotherapy response is associated with broad transcriptomic differences rather than a single molecular change.

## Candidate Biomarker Analysis

The original study selected **73 genes** for further survival analysis using external breast cancer datasets.

In the METABRIC dataset, seven genes showed statistically significant survival associations:

- TCP1
- TUBB
- C1QTNF3
- CTF1
- OLFML3
- PLA2R1
- PODN

The reported log-rank p-values ranged from less than 0.0001 to 0.011.

A separate TCGA analysis identified:

- KRT15
- HLA-A
- TCP1

as significant in that dataset.

## Cross-Dataset Validation

The original study compared its candidate gene set with another independent dataset, GSE163882.

Eleven genes were reported in common:

- C1QTNF3
- PODN
- TUBB
- MRGPRF
- PLA2R1
- KRT15
- HOXD8
- DCN
- SOD3
- SLIT3
- PRAME

Finding overlapping candidates across independent datasets is useful because it provides an additional level of evidence beyond a single discovery cohort.

## Biological Interpretation

The results suggest that chemotherapy response in breast cancer is associated with coordinated changes across multiple biological pathways.

The involvement of metabolic processes, cancer-related signalling and cell–cell communication suggests that treatment response is likely to be a complex biological phenotype.

The survival analysis also demonstrates an important research workflow:

**Differential expression → candidate prioritisation → independent survival analysis → biomarker evaluation**

However, statistical association does not establish that any individual gene directly causes chemotherapy resistance.

## Important Methodological Note

The numerical differential-expression and survival results reported here are presented as results from the original published study.

The GEO record and dataset structure were independently checked, but the published DEG and survival statistics were not presented as newly generated results from this portfolio project.

This distinction is intentional: it avoids claiming that a published result was independently reproduced when the complete count-level analysis was not executed locally.

## Limitations

Several limitations should be considered:

- The cohort contains only 22 patients.
- Patient and treatment heterogeneity may influence gene-expression patterns.
- Association does not establish causation.
- Published differential-expression results are not equivalent to independent validation.
- A stronger follow-up would reproduce the complete count-level analysis locally.
- Candidate biomarkers would require experimental and clinical validation before practical use.

## What I Learned

This project helped me understand:

- How public transcriptomic datasets can be obtained from GEO.
- Why sample groups must be defined carefully.
- Why raw RNA-seq counts require appropriate statistical methods.
- The role of DESeq2 in differential-expression analysis.
- Why multiple-testing correction is important.
- How differential-expression results can be connected to biological pathways.
- How candidate genes can be evaluated using independent datasets.
- Why reproducibility and transparent reporting are important in computational biology.

## Tools and Resources

- NCBI Gene Expression Omnibus (GEO)
- NCBI BioProject
- RNA-seq concepts
- Kallisto
- DESeq2
- Gene Ontology
- KEGG
- GSEA
- R / Bioconductor concepts

## References

- NCBI GEO: GSE162187
- NCBI BioProject: PRJNA680808
- Barrón-Gallardo CA et al. *Transcriptomic Analysis of Breast Cancer Patients Sensitive and Resistant to Chemotherapy: Looking for Overall Survival and Drug Resistance Biomarkers.*
- NCBI Gene Expression Omnibus
- NCBI Gene and Protein databases

## Conclusion

This project demonstrates a research-oriented computational biology workflow using public breast cancer transcriptomic data.

Rather than focusing only on obtaining a list of significant genes, the analysis connects differential expression with pathway interpretation, candidate biomarker selection and independent validation.

The project provided practical exposure to one of the major applications of bioinformatics: using large-scale molecular data to investigate clinically relevant biological questions.
