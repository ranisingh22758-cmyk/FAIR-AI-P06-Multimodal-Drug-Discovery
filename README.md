# P06 — FAIR-AI-P06
# Multimodal AI for Computational Drug Discovery

## Project Overview

This project develops a proof-of-concept Multimodal Artificial Intelligence framework for computational drug-discovery prioritization. It combines molecular structures, biological target information, and scientific literature to prioritize molecules for further scientific investigation.

The project investigates whether combining different types of scientific information improves predictive performance compared with single-modality models.

## Objectives

- Collect molecular activity data from ChEMBL.
- Process molecular structures using RDKit.
- Develop a Graph Convolutional Network (GCN).
- Generate scientific literature embeddings using Natural Language Processing.
- Represent biological target information using text embeddings.
- Combine molecular, target, and literature representations through multimodal fusion.
- Compare Molecular-only, Literature-only, and Multimodal models.

## Biological Target

- **Target:** Epidermal Growth Factor Receptor (EGFR)
- **ChEMBL Target ID:** CHEMBL203
- **Organism:** Homo sapiens
- **Activity Measure:** IC50

## Technologies Used

- Python 3.11
- Anaconda
- Jupyter Notebook
- Pandas and NumPy
- RDKit
- PyTorch
- PyTorch Geometric
- Scikit-learn
- Sentence Transformers
- Matplotlib

## Data Sources

- [ChEMBL](https://www.ebi.ac.uk/chembl/)
- [PubMed](https://pubmed.ncbi.nlm.nih.gov/)
- [PubChem](https://pubchem.ncbi.nlm.nih.gov/)
- [BindingDB](https://www.bindingdb.org/)
- [DeepChem](https://deepchem.readthedocs.io/)
- [MoleculeNet](https://moleculenet.org/)

ChEMBL and PubMed were used in the reported experiment. The other resources are relevant for further development.

## Experimental Results

The three approaches were evaluated using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²).

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Molecular-only GNN | 1.6072 | 1.8379 | 0.1147 |
| Literature-only | 5.1950 | 5.5501 | -7.0731 |
| Multimodal | 1.6603 | 1.8681 | 0.0854 |

The Molecular-only GNN performed best among the three evaluated approaches. In this experiment, multimodal fusion did not outperform the molecular-only baseline.

## Conclusion

The project demonstrates a proof-of-concept pipeline combining molecular graph learning, scientific text embeddings, target representation, and multimodal feature fusion. The results highlight the importance of molecule-specific literature, larger datasets, and more extensive validation.

The generated predictions are computational research-prioritization signals, not evidence of clinical efficacy or safety.

## Project Status

Academic AIML PBL project — FAIR-AI-P06.

## Future Scope

- Incorporate molecule-specific scientific literature.
- Expand the molecular activity dataset.
- Explore advanced GNN architectures.
- Improve multimodal fusion and model validation.
- Investigate ranking-based evaluation metrics.

## Author

Developed as part of the P06 AIML Project: FAIR-AI-P06 — Multimodal AI for Computational Drug Discovery.
