# Data Preprocessing and Model Training Workflow

## Overview

This project implements a workflow for preprocessing healthcare data and training machine learning models to predict hospital readmission. The dataset used is derived from the diabetic data records, with additional socioeconomic indicators integrated for richer insights. 

## Features

- **Data Preprocessing**: Handles missing values, maps categorical features, and creates socioeconomic index (SES) as a composite indicator.
- **Feature Engineering**: Derives features such as total prior visits, hierarchical encoding for diagnoses, and SES-related attributes.
- **Handling Class Imbalance**: Utilizes SMOTETomek to address imbalanced data.
- **Model Training and Evaluation**: Implements multiple classifiers (XGBoost, LightGBM, CatBoost, and AdaBoost) with learning curve visualization and ROC curve analysis.
- **Exploratory Data Analysis**: Provides insights into SES disparities and their relation to readmission rates.

## Prerequisites

- Python 3.7 or later
- Required libraries listed in `requirements.txt`

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. Ensure the dataset (`diabetic_data.csv`) and ICD-9 mapping files (`V27LONG_SHORT_DX_110909.csv`, `V27LONG_SHORT_DX_110909u021012.csv`) are in the root directory.

## Usage

1. Run the preprocessing and feature engineering steps to clean and prepare the dataset:
    ```bash
    python preprocess.py
    ```

2. Train and evaluate models using the prepared data:
    ```bash
    python train_models.py
    ```

3. Visualize results such as feature importance and SES cluster analysis:
    ```bash
    python visualize_results.py
    ```

## Results

- Insights into SES disparities among patients.
- Comparative evaluation of multiple machine learning models for readmission prediction.
- Identification of key features influencing readmission.

## Contributing

Contributions are welcome! Please open a pull request with your changes.
s
## License

This project is licensed under the MIT License. See `LICENSE` for more details.
