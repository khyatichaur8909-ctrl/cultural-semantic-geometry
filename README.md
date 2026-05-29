# Multilingual Cultural Geometry

## Overview

This repository contains the code, dataset, statistical analyses, and figures used in the study:

**Multilingual Representational Geometry of Culturally Asymmetric Concepts in Transformer Language Models**

The project investigates how multilingual transformer language models internally process culturally asymmetric concepts that do not possess direct cross-lingual semantic correspondence. Using layerwise hidden-state analysis, the study examines how culturally asymmetric Japanese concepts evolve across transformer depth compared with multiple control conditions.

## Models

* TinyLlama-1.1B-Chat-v1.0
* Qwen1.5-1.8B-Chat

## Dataset

The repository contains a dataset of 20 culturally asymmetric Japanese concepts together with control conditions.

Conditions include:

* J_asym: Japanese culturally asymmetric concepts
* E_lit: Literal English translations
* S_sym: Semantically symmetric Spanish controls
* E_base: English baseline prompts

Dataset location:

`data/culturally_asymmetric_concepts.csv`

## Repository Structure

* `notebooks/` – hidden-state extraction, statistical analysis, and figure generation notebooks
* `data/` – concept dataset
* `results/` – statistical outputs and processed results
* `figures/` – publication figures

## Reproducibility

Install dependencies:

```bash
pip install -r requirements.txt
```

Run notebooks in the following order:

1. 01_hidden_state_extraction.ipynb
2. 02_statistical_analysis.ipynb
3. 03_figure_generation.ipynb

## Analyses

The repository reproduces:

* Layerwise representational trajectory analysis
* Cosine-distance measurements
* Permutation testing
* Bootstrap confidence intervals
* ANOVA
* Effect-size estimation
* Publication figures

## Citation

If you use this repository, please cite the associated manuscript.
