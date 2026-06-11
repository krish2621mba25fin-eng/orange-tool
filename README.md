# Predictive Modeling with Orange Data Mining

An automated machine learning and data science workflow built using Orange Data Mining. This pipeline processes raw data, configures feature selection, trains a supervised classification model, and evaluates its performance metrics.

---

## 📸 Workflow Architecture

The visual pipeline establishes a clear data flow from raw files to cross-validated model evaluation.

### Supervised Learning Execution Pipeline
The entire model training and validation pipeline constructed inside Orange Data Mining:

<p align="center">
  <img src="WhatsApp Image 2026-06-11 at 1.33.59 PM.jpeg" alt="Orange Machine Learning Workflow" width="100%">
</p>

---

## ⚙️ Pipeline Components & Data Flow

The visual nodes execute the data science lifecycle in a linear, predictable sequence:

```mermaid
graph LR
    A[File Input Node] -->|Data| B[Select Columns]
    B -->|Data| C[Test and Score]
    B -->|Data| D[Logistic Regression]
    D -->|Learner| C
