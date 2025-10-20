# Vehicle Price Prediction System - Copilot Instructions

## Project Overview
This project aims to build a robust machine learning system to predict vehicle prices based on historical data. The workflow includes data preprocessing, feature engineering, model training, evaluation, and deployment. The system is designed to help users estimate the fair market value of vehicles using various attributes.

## Technology Stack
- **Language**: Python 3.x
- **Data Processing**: pandas, numpy
- **Modeling**: scikit-learn
- **Visualization**: matplotlib, seaborn
- **Notebooks**: Jupyter Notebook
- **File Storage**: CSV for data, joblib for model persistence

## Architecture Principles

### Code Organization
- Organize code by pipeline stages: preprocessing, feature engineering, modeling, evaluation
- Use modular scripts and notebooks for each stage
- Store configuration files in `models/configs/`
- Store results and outputs in `results/outputs/`
- Use strict variable naming and documentation

### File Structure Convention
```
data/
  raw/                # Raw input data
  external/           # External datasets
models/
  configs/            # Model and pipeline configs
  notebooks/          # Model training and analysis notebooks
results/
  outputs/            # Model outputs and predictions
  eda_visualizations/ # EDA plots and visualizations
notebooks/            # Preprocessing and feature engineering notebooks
```

## Data Preprocessing Guidelines

- Handle missing values using imputation strategies
- Remove outliers using statistical methods
- Encode categorical variables using label or one-hot encoding
- Normalize and scale features for model compatibility
- Save processed datasets in `results/outputs/`

## Model Training Guidelines

- Use regression algorithms (Linear Regression, Random Forest, etc.)
- Split data into training and test sets (e.g., 80/20)
- Tune hyperparameters using GridSearchCV or similar
- Evaluate models using R², RMSE, MAE
- Save trained models using joblib in `results/outputs/`
- Document model parameters and performance

## Feature Engineering Guidelines

- Select relevant features using statistical tests or model-based selection
- Create new features if beneficial (e.g., age of vehicle)
- Store feature selection results in `results/outputs/`

## Visualization Guidelines

- Use matplotlib/seaborn for EDA and model evaluation plots
- Save visualizations in `results/eda_visualizations/`
- Plot feature importance, residuals, and prediction comparisons

## Security Guidelines

- Validate all input data for type and range
- Sanitize file uploads and outputs
- Use environment variables for sensitive paths if needed

## Model Evaluation Guidelines

- Compare multiple models and select the best based on metrics
- Use cross-validation for robust performance estimation
- Document evaluation results in notebooks and output files

## File Management

- Store all intermediate and final datasets in `results/outputs/`
- Use clear naming conventions for files (e.g., `final_output.csv`, `scaled_data.csv`)
- Version control for model and data files

## Testing Strategy

- Test data preprocessing steps for correctness
- Validate model predictions on test data
- Ensure reproducibility by fixing random seeds

## Compliance and Standards

- Follow best practices for machine learning projects
- Document all steps and decisions in notebooks
- Ensure code readability, maintainability and simplicity
- Write each method/step in a seperate cell
- Provide comments where necessary
- Do not use emojies in the code
- Always ask permission to implement code before implementing it yourself