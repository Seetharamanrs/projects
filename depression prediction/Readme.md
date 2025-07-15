# Student Depression Severity Detection

This project applies machine learning techniques to predict the severity of depression among students based on behavioral, academic, and social factors. With mental health becoming an increasingly critical issue in academic environments, this project aims to support early identification and intervention using data-driven methods.

##  Objective

- Predict depression severity among students using supervised machine learning models.
- Identify the most relevant features affecting mental health.
- Compare model performance across traditional and deep learning algorithms.
- Provide interpretability and actionable insights for educational and clinical stakeholders.

##  Background

Traditional diagnostic methods often struggle to capture the complexity of mental health issues. This project leverages supervised learning algorithms to provide a scalable, data-driven approach to detect varying levels of depression severity among students, with a focus on interpretability and real-world application.

## Dataset

- Source: Nguyen et al. (2019) – includes student mental health, academic stress, social behaviors, and cultural factors.
- Size: ~285 records (after cleaning)
- Target: Depression Severity (`DepSev`)
- Features: Academic pressure, family background, social connectivity, help-seeking behavior, etc.

##  Methods

- **Data Preprocessing**: Label encoding, feature correlation analysis, and outlier removal.
- **Feature Selection**: Based on correlation thresholds (0.1 and 0.2).
- **Models Used**:
  - Random Forest
  - Support Vector Machine (SVM)
  - Neural Network (Keras Sequential)
  - Ensemble Voting Classifier (RF + SVM)

## Results

| Model            | Accuracy | F1 Score | AUC-ROC |
|------------------|----------|----------|---------|
| Random Forest    | 95.06%   | 0.93     | 0.995   |
| Neural Network   | 94.85%   | 0.92     | ~0.98   |
| SVM              | 91.0%    | 0.89     | ~0.93   |

> Best results achieved with Random Forest using a feature correlation threshold of 0.2 and 5-class classification (Depression Severity levels).

##  Key Insights

- **Academic stress**, **social isolation**, and **family background** were found to be top predictors.
- Feature selection significantly improved model performance and interpretability.
- Cross-validation helped mitigate overfitting and improved model robustness.

##  Limitations

- Dataset is cross-sectional and based on self-reported responses.
- Lacks external validation on clinical populations.
- May not generalize across demographics without larger, more diverse datasets.

##  Future Work

- Incorporate longitudinal and multi-institutional data.
- Expand to multimodal inputs (text, voice, activity).
- Improve model interpretability using tools like SHAP or LIME.

##  Tech Stack

- Python (Pandas, NumPy, Scikit-learn, TensorFlow/Keras, Seaborn, Plotly)
- Jupyter Notebook
- Google Colab
##  Acknowledgements

- Dataset: Nguyen et al. (2019) – Mental Health and Help-Seeking Behavior of Students
- Referenced studies: Haque et al. (2021), Shin et al. (2020), Nemesure et al. (2021), etc.


---

**Disclaimer:** This project is for educational and research purposes only. It is not intended for clinical use or diagnosis.
