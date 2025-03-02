# Loan Risk Assessment using Explainable AI (XAI)

This project leverages machine learning techniques to predict loan approvals while providing transparent explanations using SHAP (SHapley Additive exPlanations). The goal is to ensure fairness by highlighting key financial factors influencing loan decisions. A live demonstration of the model is available through a Streamlit web application: [Loan Risk Assessment App](https://loan-risk-assessment-using-xai.streamlit.app/).

## Overview

In the financial sector, the transparency of AI-driven decisions is crucial for building trust and ensuring compliance with regulatory standards. This project addresses this need by integrating explainable AI techniques into the loan approval process. By utilizing SHAP values, the model not only predicts loan approvals but also provides clear insights into the factors influencing each decision.

## Features

- **Predictive Modeling**: Utilizes machine learning algorithms to assess loan applications.
- **Explainability**: Implements SHAP to offer transparent explanations for each prediction.
- **Web Application**: Interactive interface for users to input data and receive predictions with explanations.

## Dataset

The dataset used in this project is `Loan.csv`, which contains anonymized loan application data with various financial attributes. This dataset is essential for training and evaluating the predictive model.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Chiugo-Nsoke/Loan-Risk-Assessment-using-XAI.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd Loan-Risk-Assessment-using-XAI
   ```

3. **Create a virtual environment** (optional but recommended):

   ```bash
   python -m venv env
   ```

4. **Activate the virtual environment**:

   - On Windows:
     ```bash
     env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

5. **Install the required packages**:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

After installation, you can run the web application locally:

```bash
streamlit run app.py
```

This command will launch the Streamlit app, allowing you to input loan application data and receive predictions along with SHAP-based explanations.

## File Structure

The repository comprises the following key files and directories:

- `Loan.csv`: The dataset containing loan application records.
- `Risk Project-Copy3.ipynb`: Jupyter Notebook detailing the data analysis, model training, and evaluation processes.
- `app.py`: Streamlit application script for the interactive web interface.
- `loan_approval_model.pkl`: Serialized machine learning model for predicting loan approvals.
- `Scaler.pkl`: Serialized scaler object used for data normalization.
- `requirements.txt`: List of Python dependencies required to run the project.
- `.devcontainer/`: Configuration files for development container setup.

## Explainable AI Techniques

This project employs SHAP values to interpret the predictions made by the machine learning model. SHAP provides a unified measure of feature importance, allowing for both global and local interpretability:

- **Global Interpretability**: Understanding which features most influence the model's overall predictions.
- **Local Interpretability**: Explaining the factors that led to a specific prediction for an individual loan application.

By integrating SHAP, the project ensures that stakeholders can comprehend the rationale behind each loan approval decision, promoting transparency and trust.

## Contributing

Contributions to enhance the project are welcome. To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Make your changes.
4. Commit your changes:
   ```bash
   git commit -m 'Add some feature'
   ```
5. Push to the branch:
   ```bash
   git push origin feature-branch-name
   ```
6. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
