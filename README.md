
# OncoInsight-AI
## Explainable Machine Learning for Breast Cancer Classification

### Project Overview
OncoInsight-AI is a bioinformatics and machine learning project
that applies supervised learning and explainable AI to classify
breast cancer samples as benign or malignant.

The project uses the Breast Cancer Wisconsin Diagnostic dataset
from Scikit-learn.

### Dataset
- Total samples: 569
- Features: 30 numerical features
- Benign samples: 357
- Malignant samples: 212
- Missing values: None

The features describe characteristics of cell nuclei obtained
from digitized fine needle aspirate images.

### Methodology
1. Data loading and preprocessing
2. Exploratory data analysis
3. Correlation analysis
4. Train-test splitting (80:20)
5. Logistic Regression classification
6. Random Forest classification
7. Five-fold stratified cross-validation
8. Feature importance analysis
9. SHAP explainability

### Model Performance

| Model | Test Accuracy | Test ROC-AUC |
|---|---:|---:|
| Logistic Regression | 98.25% | 0.9954 |
| Random Forest | 94.74% | 0.9937 |

### Cross-validation Results

| Model | Mean Accuracy | Mean ROC-AUC |
|---|---:|---:|
| Logistic Regression | 97.80% | 0.9959 |
| Random Forest | 96.26% | 0.9923 |

### Important Predictive Features
- Worst perimeter
- Worst area
- Worst concave points
- Mean concave points
- Worst radius
- Worst texture

### Explainable AI
SHAP was used to investigate feature contributions to
malignant probability predictions.

### Biological Interpretation
Nuclear size, shape, concavity and texture measurements
contributed to the classification of benign and malignant
samples in this dataset.

These are morphological predictive features, not gene-expression
biomarkers.

### Repository Structure
- results/figures/: Analysis figures and visualizations
- results/tables/: Model performance and feature importance tables

### Tools and Technologies
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SHAP

### Limitations
This project uses a single train-test split and five-fold
cross-validation on the training data. Results are dataset-specific
and do not establish clinical diagnostic performance.

### Future Scope
- External validation using an independent dataset
- Integration of public breast cancer gene-expression data
- Molecular biomarker discovery
- Further explainability and model validation

### Disclaimer
This is an educational and research portfolio project.
It is not intended for clinical diagnosis or medical decision-making.
