# NBA-Player-Statistical-Analysis-and-Classification-Engine

## Project Overview
This project encapsulates a robust machine-learning framework designed to classify NBA players into one of five basketball court positions (SG, PG, SF, PF, C) based on their per-game performance statistics during the regular season. Utilizing a sophisticated feature engineering process and advanced machine learning algorithms, this system offers high precision in predicting player roles from complex statistical data.

## Data Description
The dataset comprises per-game player statistics sourced from the NBA's regular season, structured in a tabular format within a "nba_stats.csv" file. These statistics include a myriad of performance indicators such as points per game (PPG), assists per game (APG), rebounds per game (RPG), among others.

## Technical Specifications
- **Data Preprocessing:** The preprocessing pipeline employs techniques such as normalization, imputation of missing values, and reduction of dimensionality through correlation analysis and feature selection based on predictive value.
- **Machine Learning Model:** The classification model is built using the Support Vector Machine (SVM) algorithm with a radial basis function (RBF) kernel. This choice is driven by SVM's efficacy in handling high-dimensional data and its capacity to model non-linear decision boundaries.
- **Model Evaluation Strategy:** Model robustness is verified through a rigorous evaluation strategy that includes a hold-out validation set, a separate dummy test set, and a 10-fold stratified cross-validation to ensure the model's effectiveness and generalizability across various subsets of data.

## Installation Requirements
This project is implemented in Python, requiring the following libraries: NumPy, Pandas, Scikit-learn, Matplotlib, and Seaborn. You can install these dependencies using pip:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```
## Running the Project
1. Ensure that the dataset files nba_stats.csv and dummy_test.csv are in the same directory as the script.
2. Run the script using Python. For example:
    ```bash
   python nba_classification.py
   ```
## Outputs
The system outputs several key metrics:
-Accuracy scores for the training and validation datasets.
-Confusion matrices for the training, validation, and dummy test datasets, providing detailed insights into class-specific performance.
-Accuracies for each fold in the cross-validation process, alongside the computation of the mean cross-validation accuracy.

## License
This project is released under the MIT License, which provides extensive rights to modify and reuse the software.
