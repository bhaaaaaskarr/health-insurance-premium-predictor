# Health Insurance Premium Predictor

## Overview
The Health Insurance Cost Predictor is a Streamlit-based web application that estimates the cost of health insurance based on user inputs. It utilizes machine learning models trained on various health and demographic factors to provide accurate predictions.

## Features
- User-friendly Streamlit interface
- Input fields for various user attributes, including age, income, BMI category, smoking status, medical history, and more
- Predicts insurance cost using trained machine learning models
- Normalizes risk scores based on medical history
- Uses different models for younger and older individuals

## Tech Stack
- **Frontend**: Streamlit
- **Backend**: Python
- **Machine Learning**: Scikit-learn, Joblib
- **Data Processing**: Pandas, NumPy

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- pip

### Steps
1. Clone the repository:
   ```sh
   git clone    git clone https://github.com/your-repo/health-insurance-predictor.git

   cd health-insurance-predictor
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the application:
   ```sh
   streamlit run app.py
   ```

## Usage
1. Open the Streamlit application in your browser.
2. Fill in the input fields with relevant details.
3. Click the "Predict" button to get the estimated insurance cost.

## Project Structure
```plaintext
├── artifacts/
│   ├── model_young.joblib
│   ├── model_old.joblib
│   ├── scaler_young.joblib
│   ├── scaler_old.joblib
├── app.py
├── prediction_helper.py
├── requirements.txt
├── README.md
```
- **`app.py`**: Main Streamlit application
- **`prediction_helper.py`**: Contains functions for preprocessing and prediction
- **`artifacts/`**: Stores trained models and scalers
- **`requirements.txt`**: List of dependencies

## Model Details
The project uses two separate models:
- `model_young.joblib`: For individuals aged 25 and below
- `model_old.joblib`: For individuals above 25

Both models are trained on various demographic and medical factors to estimate insurance costs.

## Acknowledgments
This project was built as part of a machine learning application for predicting health insurance costs. Special thanks to the open-source community for the tools and resources used in this project.

## License
This project is licensed under the MIT License.

---
Feel free to contribute by submitting issues or pull requests!

