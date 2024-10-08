# Dataset Description

This document provides a detailed description of the datasets included in the **Once Learning Document Dataset** repository. The dataset is organized into two primary categories, **One-Page Document Comparisons** and **Multi-Page Document Comparisons**, each designed to evaluate different aspects of a model’s ability to recognize and understand visual patterns.

## 1. One-Page Document Comparisons

### Overview

The **One-Page Document Comparisons** dataset contains document pairs, each consisting of a single page. The focus is on evaluating a model's ability to identify whether the patterns in these single-page documents share the same structure or not.

### File: `one_page_document_comparisons.csv`

- **Description**: This file contains comparisons between different single-page documents, each from a unique pattern category. It helps assess whether models can accurately differentiate between patterns in single-page scenarios.
- **Columns**:
  - **`file1`**: Path to the first document in the comparison (e.g., `pattern00\\gnmm0220.tif`).
  - **`file2`**: Path to the second document in the comparison (e.g., `pattern01\\fjcj0179.tif`).
  - **`same_pattern`**: Binary value indicating if both documents share the same pattern (`1`) or not (`0`).

### Example Rows from `one_page_document_comparisons.csv`

| Index | file1                     | file2                     | same_pattern |
|-------|---------------------------|--------------------------|--------------|
| 2     | pattern00\\gnmm0220.tif     | pattern01\\fjcj0179.tif    | 0            |
| 3     | pattern00\\gnmm0220.tif     | pattern01\\gkdj0179.tif    | 0            |
| 4     | pattern00\\gnmm0220.tif     | pattern01\\hkdj0179.tif    | 0            |
| 5     | pattern00\\anmm0220.tif     | pattern01\\inxp0179.tif    | 0            |

### Usage

- **Same Pattern Comparison**: A `1` in the `same_pattern` column indicates that the two documents in the comparison share the same pattern, based on their structural properties.
- **Different Pattern Comparison**: A `0` in the `same_pattern` column indicates that the two documents in the comparison belong to different patterns or categories.

### Purpose

This dataset allows researchers to test a model's performance in recognizing patterns within individual pages. The differentiation between same and different patterns is crucial in evaluating the model’s generalization ability with minimal visual information.

---

## 2. Multi-Page Document Comparisons (To be added)

### Overview

The **Multi-Page Document Comparisons** dataset (yet to be added) will focus on evaluating a model’s ability to understand and identify patterns across multiple pages. This includes tasks like cross-page relationships, sequential patterns, and references.

---

### Additional Information

As the dataset evolves, new types of comparisons and documents will be added. Please refer to this document for the latest updates on dataset structure and content.