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

# Results and Metrics for LLM Models

### Confusion Matrix - GPT-4o-mini

| True Value \ Predicted | Predicted 0 | Predicted 1 |
|------------------------|-------------|-------------|
| **True 0**             | 10           | 0           |
| **True 1**             | 10           | 0           |

 **Precision**  0.00  
 **Recall**     0.00  
 **F1-score**   0.00  
 **Accuracy**   0.50  

### Confusion Matrix - GPT-4o

| True Value \ Predicted | Predicted 0 | Predicted 1 |
|------------------------|-------------|-------------|
| **True 0**             | 10           | 0           |
| **True 1**             | 10           | 0           |

 **Precision**  0.00  
 **Recall**     0.00  
 **F1-score**   0.00  
 **Accuracy**   0.50  

### Confusion Matrix - GPT-4 Turbo

| True Value \ Predicted | Predicted 0 | Predicted 1 |
|------------------------|-------------|-------------|
| **True 0**             | 8           | 2           |
| **True 1**             | 9           | 1           |

 **Precision**  0.33  
 **Recall**     0.10  
 **F1-score**   0.15  
 **Accuracy**   0.45  

### Confusion Matrix - LLaMA 3.2 11B Vision Instruct

| True Value \ Predicted | Predicted 0 | Predicted 1 |
|------------------------|-------------|-------------|
| **True 0**             | 8           | 2           |
| **True 1**             | 7           | 3           |

 **Precision**  0.60  
 **Recall**     0.30  
 **F1-score**   0.40  
 **Accuracy**   0.55  


### Observations:
- The cell `True 0 | Predicted 0` shows the true negatives (cases where the pattern was 0 and the model correctly predicted 0).
- The cell `True 1 | Predicted 1` shows the true positives (cases where the pattern was 1 and the model correctly predicted 1).
- The cell `True 0 | Predicted 1` shows the false positives (cases where the pattern was 0, but the model predicted 1).
- The cell `True 1 | Predicted 0` shows the false negatives (cases where the pattern was 1, but the model predicted 0).

These values can be used to calculate metrics such as precision, recall, F1-score, and accuracy for each model.

