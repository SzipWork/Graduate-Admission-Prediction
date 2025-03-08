# Graduate Admission Prediction

## Overview
This project predicts a student's likelihood of admission into a graduate program based on academic and test scores. It utilizes **machine learning regression models** to analyze key admission factors.

## Dataset
- **Source:** Graduate Admission Dataset
- **Features:** GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research Experience
- **Target Variable:** Chance of Admission (0 to 1)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/graduate-admission-prediction.git
   cd graduate-admission-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Model Training
1. **Data Preprocessing:** Handling missing values, feature scaling, and data normalization.
2. **Model Used:** Linear Regression, Random Forest, or Ridge Regression.
3. **Evaluation Metrics:** Mean Squared Error (MSE), R² Score.
4. **Model Saving:** Trained model is saved using Pickle (`admission_model.pkl`).

## Usage
- Load the trained model:
  ```python
  import pickle
  model = pickle.load(open('admission_model.pkl', 'rb'))
  ```
- Make predictions:
  ```python
  sample_data = [[320, 110, 4, 4.5, 4.0, 9.0, 1]]  # Example input
  predicted_chance = model.predict(sample_data)
  print(predicted_chance)
  ```

## Results & Improvements
- Achieved high prediction accuracy for graduate admissions.
- Possible improvements: Feature engineering, hyperparameter tuning, and deep learning models.
