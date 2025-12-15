# Mlflow-Red-Neuronal-Fine-Tuning

## Description of the Problem
In supervised classification tasks, achieving a good balance between precision and recall
is often more relevant than maximizing accuracy alone. Base neural network models may
present acceptable accuracy values but fail to generalize correctly across classes,
especially when the data distribution is not perfectly balanced.

This project addresses the problem of improving classification performance through
systematic fine-tuning of a neural network model, using MLflow to track experiments,
compare configurations, and support objective model selection.



## Technology Stack
- **Programming Language:** Python
- **Machine Learning:** Scikit-learn, TensorFlow / Keras
- **Experiment Tracking:** MLflow
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib
- **Environment:** Jupyter Notebook



## Architecture – Phased Approach

The solution follows a phased experimental architecture:

### Phase 1 – Base Model
A baseline neural network model is trained and evaluated to establish a reference
performance level.

### Phase 2 – Optimized Models
Previously optimized configurations are evaluated and compared against the base model.

### Phase 3 – Systematic Fine-Tuning
Multiple fine-tuning configurations are defined by adjusting hyperparameters such as:
- Learning rate
- Network configuration
- Training parameters

Each configuration is logged as an independent experiment in MLflow.

### Phase 4 – Evaluation and Comparison
All models are evaluated using multiple metrics, allowing a comprehensive comparison
based on overall classification performance.



## Captures
- MLflow experiment tracking interface
- Metric comparison across configurations
- Model performance summaries

Visual evidence of these results can be found in:
- `SolanoAGuillenJ_MlflowFineTuningV1.html`
- `Resultados_SolanoAGuillenJ_MlflowFineTuningV1.pdf`



## What Was Achieved
- Implementation of a reproducible fine-tuning workflow
- Centralized experiment tracking using MLflow
- Objective comparison of multiple neural network configurations
- Identification of a fine-tuned model with improved overall performance balance



## Code
The full implementation is available in the following files:

- **`SolanoAGuillenJ_MlflowFineTuningV1.ipynb`**  
  Contains the complete experimental pipeline, including model definition, training,
  fine-tuning configurations, MLflow logging, and evaluation.

- **`SolanoAGuillenJ_MlflowFineTuningV1.html`**  
  Executed and exported version of the notebook for direct visualization.



## Quantifiable Results
- Accuracy values remained stable across configurations (approximately 0.78–0.80),
  indicating limited sensitivity to hyperparameter changes.
- The F1-score showed clearer performance differences between models.
- One systematic fine-tuning configuration achieved the highest F1-score, outperforming
  both the base model and previously optimized versions.
- Precision and recall were better balanced in the selected fine-tuned model, improving
  overall classification reliability.

Detailed numerical results and analysis are documented in
`Resultados_SolanoAGuillenJ_MlflowFineTuningV1.pdf`.



## Authors
Ariel Solano  
Juan Guillén  

Universidad Politécnica Salesiana  
Artificial Intelligence – Integrative Practice  
December 2025
