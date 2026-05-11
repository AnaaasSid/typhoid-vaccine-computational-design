# typhoid-vaccine-computational-design
Computational immunoinformatics pipeline for the identification of potential B-cell and T-cell epitopes in Salmonella Typhi FliC flagellin.
# Multi-Epitope Vaccine Design for Salmonella Typhi 🧬

## Project Overview
This repository contains a computational biology workflow dedicated to the reverse vaccinology of **Salmonella Typhi**. The primary focus is the **FliC/FljB family flagellin protein** (Accession: WP_000079784.1), an essential factor for bacterial motility and a potent trigger for the host immune response.

## 🛠 Immunoinformatics Pipeline
The selection process followed a rigorous four-stage screening protocol:
1. **Sequence Retrieval:** Extraction of the flagellin protein sequence in FASTA format.
2. **Antigenicity Assessment:** Utilizing **VaxiJen v2.0** (Bacteria Model) with a threshold of > 0.4 to identify probable antigens.
3. **Epitope Prediction:** Utilizing **BepiPred** and surface accessibility metrics.
4. **Safety Profiling:** Screening candidates via **AllerTOP** to ensure non-allergenicity and low toxicity.

## 📊 Key Results & Candidates
The pipeline identified high-ranking B-cell epitope candidates based on their antigenic scores:

| Epitope ID | Sequence | VaxiJen Score | Status |
| :--- | :--- | :--- | :--- |
| **B_Epi_1** | `NKSQSALGTAIERLSSGLRINSAKD` | 0.7376 | Probable Antigen |
| **B_Epi_2** | `ANGTNSQSDLDS` | **1.4000** | **High Efficacy Candidate** |
| **B_Epi_3** | `LGNTVNNLSSARSRIEDSD` | 0.5199 | Probable Antigen |

## 📁 Repository Structure
- `Typhoid_Vaccine_Project.ipynb`: The primary computational ledger containing Python-based data logging and results.
- `typhi_flic.fasta`: The raw protein sequence used for analysis.

## 🚀 Future Scope
Further stages of this project include **T-Cell Epitope Prediction**, **MHC-II Allele Binding analysis**, and **Molecular Docking** simulations to validate binding affinity with human immune receptors.
