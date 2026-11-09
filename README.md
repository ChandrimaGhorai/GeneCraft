# GeneCraft 🧬

GeneCraft is an automated bioinformatics pipeline designed to process reference and sample DNA sequences in a single pass. It eliminates the manual stitching of multiple tools by combining translation, biophysical profiling, and functional mutation classification into a unified, reproducible workflow.

## Key Features

- **Automated Translation:** Automatically transcribes DNA/mRNA into functional protein profiles and handles stop codons seamlessly.
- **Start-Codon Validation:** Locates valid `ATG` start codons and tracks their 0-indexed positions accurately regardless of sequence placement.
- **Biophysical Profiling:** Computes critical metrics including GC content, melting temperature ($T_m$), molecular weight, net charge, and GRAVY hydropathy scores.
- **Precise Mutation Classification:** Categorizes functional consequences based on robust biological rules (silent, missense, nonsense, frameshift, or in-frame indels).
- **Proactive Warnings:** Flags structural risks such as residue rigidity shifts, disrupted prolines, or percentage-based ORF truncation.

## Workflow Overview

1. **Input:** User supplies a reference sequence and a sample sequence suspected of carrying a mutation.
2. **Processing:** Sequences are transcribed against a standard codon table and translated into proteins, with 0-indexed start codons tracked.
3. **Biophysical & Structural Evaluation:** Stability figures and structural metrics are evaluated on both nucleic acid and amino acid levels.
4. **Diagnostic Reporting:** Functional impacts are categorized and bundled into an automated report.

## Usage

You can run the complete analysis pipeline interactively via Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ffxqAoFPt2_mbesLrehKtJeIosxgsjHj?usp=sharing)
