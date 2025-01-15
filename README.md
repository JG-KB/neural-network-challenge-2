
# Attrition and Department Prediction

This project implements a neural network model to predict employee attrition and department using TensorFlow/Keras. 
It processes a dataset with various features and builds a branched neural network to predict these two outputs.

## Project Overview

### **1. Preprocessing**
- **Data Import**: Imports the dataset and necessary libraries.
- **Feature Selection**: Selects 10 features from the dataset for the X variables.
- **Target Variables**: Creates a DataFrame with 'Attrition' and 'Department' columns.
- **Encoding**: Encodes categorical data using `OneHotEncoder`.
- **Scaling**: Standardizes the numeric features using `StandardScaler`.
- **Train-Test Split**: Splits the dataset into training and testing sets.

### **2. Model Development**
- **Architecture**: Creates a branched neural network model:
  - Shared layers for general feature processing.
  - Separate branches for 'Attrition' and 'Department' predictions.
- **Loss Functions**: Uses `categorical_crossentropy` for 'Department' and `binary_crossentropy` for 'Attrition'.
- **Training**: Trains the model for 100 epochs using `adam` optimizer.

### **3. Evaluation**
- Evaluates the model on the testing dataset.
- Outputs accuracy for both 'Attrition' and 'Department'.

## Project Structure
- **`attrition.ipynb`**: Jupyter Notebook containing all the code, from preprocessing to evaluation.
- **Preprocessing Steps**:
  - Encode categorical variables.
  - Scale numeric features.
- **Model**:
  - Input layer processes 10 features.
  - Two shared dense layers.
  - Two branches: 'Attrition' and 'Department'.
- **Evaluation**:
  - Outputs accuracy for both targets.

## Installation
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook.

## Usage
- Open `attrition.ipynb` in Jupyter Notebook or VSCode.
- Run all cells to preprocess data, train the model, and evaluate performance.

## Results
- Department Prediction Accuracy: ~81%
- Attrition Prediction Accuracy: ~50%

## Future Improvements
- Address data imbalance for 'Attrition' using SMOTE or class weights.
- Perform feature selection to reduce noise.
- Use advanced architectures like batch normalization and dropout for better generalization.
- Tune hyperparameters using grid search or Optuna.

## Questions
For any questions or suggestions, feel free to reach out!
