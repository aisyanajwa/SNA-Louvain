# Toward Personalized Dating Recommendations: Graph-Based Community Detection Using Louvain and Cosine Similarity on OkCupid

Code and experimental artifacts for the paper published in the **2026 International Conference on Information Technology and Computing (ICITCOM)**.

- **DOI**: [10.1109/ICITCOM70739.2026.11714419](https://doi.org/10.1109/ICITCOM70739.2026.11714419)

## Overview

This repository contains the data preprocessing pipeline, network construction, and community detection implementation for clustering OkCupid user profiles. The framework models user attribute similarity using Cosine Similarity ($\theta > 0.70$) and partitions the resulting network using the Louvain algorithm with a deterministic seed (`random_state=4082`).

The experiments include:
- Graph construction and topological network analysis (modularity $Q = 0.6861$).
- Benchmark comparison across clustering algorithms (Louvain, Leiden, Label Propagation, Greedy Modularity / CNM, Infomap).
- Cosine threshold sensitivity analysis ($\theta \in [0.5, 0.9]$).
- Statistical significance evaluation (Chi-square and ANOVA) and attribute hold-out validation.

## Dataset

The analysis uses the OkCupid Profiles dataset:
- Source: [OkCupid Profiles on Kaggle](https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles)

To run the notebook, download `okcupid_profiles.csv` from Kaggle and place it in the `data/` directory.

## Repository Structure

```
.
├── data/
│   └── README.md                                   # Dataset link & instructions
├── notebooks/
│   └── okcupid_community_detection_louvain.ipynb   # Main analysis notebook
├── results/
│   ├── algorithm_comparison.csv                    # Modularity & runtime benchmarks
│   ├── community_size_distribution.csv             # Size of detected communities
│   ├── fig4_heatmap.png                            # Feature characteristic heatmap
│   ├── holdout_validation.csv                      # Attribute hold-out evaluation
│   ├── karakteristik_komunitas.csv                 # Feature proportions per community
│   ├── network_statistics.csv                      # Network density, clustering, modularity
│   ├── statistical_significance.csv                # Chi-Square test statistics
│   └── threshold_sensitivity.csv                   # Cosine similarity threshold sweep
├── requirements.txt
└── README.md
```

## Citation

```bibtex
@INPROCEEDINGS{11714419,
  author={Najwa, Aisya Mufidah and Alifah, Amalia Nur and Alifianti, Tarisma Dwi Putri and Pradana, Ikfan Putra Maesru Dwi},
  booktitle={2026 International Conference on Information Technology and Computing (ICITCOM)}, 
  title={Toward Personalized Dating Recommendations: Graph-Based Community Detection Using Louvain and Cosine Similarity on OkCupid}, 
  year={2026},
  volume={},
  number={},
  pages={329-334},
  keywords={Social networking (online);Aging;Printing;Labeling;Algorithms;Signal detection;Joining processes;Indexes;Indexing;Seeds (agriculture);community detection;dating apps;Louvain algorithm;cosine similarity;social network analysis},
  doi={10.1109/ICITCOM70739.2026.11714419}}
```
