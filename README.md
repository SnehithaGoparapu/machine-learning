# Project: Supply Chain AI Agent 
An end-to-end Machine Learning and Generative AI project for inventory optimization, demand forecasting, and decision support using real transactional retail data. The application combines classical forecasting, ML models, and a GenAI assistant into an interactive Streamlit dashboard.
# Project Overview
This project simulates a smart supply chain analyst that can:
Analyze historical sales transactions.
Forecast product demand.
Optimize inventory decisions (safety stock, reorder point).
Compare ML models (Random Forest vs Neural Network).
Answer natural language business questions using Google Gemini (GenAI).
Generate automated Word reports for stakeholders.
# Architecture & Workflow
1. Data Ingestion
Upload raw retail transaction data (CSV)
 2. Data Processing
Cleans invalid transactions
Aggregates sales at daily & product level
Selects top-selling products
 3. Forecasting (Time Series)
Prophet for demand forecasting
 4. Machine Learning Models
Random Forest Regressor
Neural Network (MLP Regressor)
Lag-based feature engineering
RMSE-based model comparison
 5. Inventory Optimization
Current Stock, Safety stock calculation, Reorder point estimation, Recommended order quantity
 6. GenAI Layer (Gemini)
Conversational analytics
Business-friendly insights from dataset context
 7. Visualization & Reporting
Interactive Plotly charts
Auto-generated Word reports
# Project_Folder
├── app.py            # Main Streamlit application
 
├── app.ipynb         # Jupyter Notebook for Expirements and Model logic
 
├── Dataset_csv_01    # Sample retail dataset

├── Requirements.txt  # Python dependencies

Do not rename any files.
# Environment Setup
Python version required: Python 3.9 or above
# Install Dependencies
Run the following command inside the project folder:

pip install -r Requirements.txt / pip install streamlit pandas numpy prophet google-generativeai python-docx scikit-learn plotly


This will install all required libraries including:
Streamlit, Prophet, Scikit-learn, Plotly, and others.
# Dataset Preparation

The provided dataset is:

Dataset_csv_01

Keep Dataset_csv_01 in the same project folder
# Running the code in python environment (app.py)

Run the following command in a New Terminal:

python -m streamlit run app.py / streamlit run app.py

The application will automatically open in a browser at:
http://localhost:8501

# How to Use the Application
1. Upload Dataset_csv_01 file using the sidebar

2. (Optional) Enter a Google Gemini API key

3. Select a product from the dropdown

4. Review:
   - Historical sales
   - Forecast results
   - Machine learning predictions
   - Inventory optimization metrics

6. Use the chat interface for analysis

7. Generate and download the Word report if required
# Notes for Evaluation
- If no Gemini API key is provided, the GenAI chat feature will be disabled

- All forecasting, machine learning, and optimization features will still run correctly

- Forecasting model: Prophet

- ML models: Random Forest Regressor, Neural Network (MLP)

- Evaluation metric: RMSE
# Notebook Execution 
To review experiments and model logic:

jupyter notebook: app.ipynb

Following the above steps will allow successful execution and verification of the project.
