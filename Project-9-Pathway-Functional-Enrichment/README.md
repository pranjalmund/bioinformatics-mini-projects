# Project 9 — Pathway & Functional Enrichment Analysis

## Interpreting transcriptomic signals associated with chemotherapy response in breast cancer

### Research Question

What biological processes and signaling pathways are associated with transcriptomic differences between chemotherapy-sensitive and chemotherapy-resistant breast cancer patients?

---

## 1. Project Overview

This project builds on Project 8 and moves from a differential-expression gene list toward biological interpretation.

A large list of differentially expressed genes can be difficult to interpret individually. Functional enrichment analysis helps organize these genes into biological processes and signaling pathways that may provide a broader picture of the biology associated with chemotherapy response.

The project focuses on Gene Ontology (GO), KEGG pathway interpretation, and protein-association analysis.

---

## 2. Dataset

- **GEO accession:** GSE162187
- **BioProject:** PRJNA680808
- **Organism:** Homo sapiens
- **Experiment:** RNA-seq gene-expression profiling
- **Total patient profiles:** 22
- **Chemotherapy-sensitive:** 9
- **Chemotherapy-resistant:** 13
- **Reference genome:** GRCh38
- **Differentially expressed genes reported by the original study:** 1,985

---

## 3. Biological Question

The main question was:

> What biological processes and pathways are represented among genes associated with chemotherapy response?

Rather than asking only which individual genes are differentially expressed, this project asks whether those genes form meaningful biological patterns.

---

## 4. Computational Framework

The original study used a multi-stage computational workflow:

```text
RNA-seq data
      ↓
Transcript quantification
      ↓
Differential expression analysis
      ↓
Differentially expressed genes
      ↓
GO enrichment
      ↓
KEGG pathway analysis
      ↓
GSEA
      ↓
Protein-association analysis
      ↓
Biological interpretation
