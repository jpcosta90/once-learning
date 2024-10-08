# Once Learning Benchmark for Document Analysis

## Overview
This repository provides the first benchmark dataset for evaluating models on the **Once Learning** paradigm in document analysis. Once Learning aims to evaluate a model's ability to understand and recognize patterns from a single visual instance, simulating human-like cognitive learning processes. The benchmark includes a diverse set of document patterns, each representing unique visual structures that challenge a model's generalization capabilities.

## Repository Structure
- **`docs/`**: Detailed documentation of the benchmark and methodology.
- **`data/`**: Dataset and processed data for benchmarking.
- **`files/`**: Contains all additional resources required for benchmarking, including documents, images, and other related files used in experimental evaluations.
- **`models/`**: Configurations and weights of baseline models.
- **`scripts/`**: Scripts for data preprocessing, model training, and evaluation.
- **`notebooks/`**: Jupyter notebooks for interactive experimentation.
- **`results/`**: Baseline results and evaluation plots.

## Dataset
The Once Learning Dataset consists of various tasks patterns, including:
- `One-Page-Document`: This category includes document patterns where each document consists of a single page only.
- `Multi-Page-Document`: This category includes document patterns where the understanding of the content requires analyzing multiple pages together.

Detailed dataset description can be found in [docs/dataset_description.md](docs/dataset_description.md).

## Getting Started
1. **Clone the repository:**
   ```bash
   git clone https://github.com/username/once-learning.git
