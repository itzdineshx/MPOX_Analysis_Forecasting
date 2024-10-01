# **Monkeypox (MPOX) Case Analysis and Forecasting Using Time Series Models**

### **Project Overview**
This project involves a comprehensive analysis and time series forecasting of global Monkeypox (MPOX) cases during the 2022-2024 outbreak. The analysis leverages historical data and employs advanced time series models such as ARIMA and SARIMA to predict future trends in Monkeypox cases. The results aim to provide valuable insights into the outbreak's trajectory and inform public health strategies.

### **Table of Contents**
1. [Introduction](#introduction)
2. [Project Objectives](#project-objectives)
3. [Data Sources](#data-sources)
4. [Methodology](#methodology)
5. [Results and Visualizations](#results-and-visualizations)
6. [Project Structure](#project-structure)
7. [How to Run the Project](#how-to-run-the-project)
8. [Dependencies](#dependencies)
9. [Limitations and Future Work](#limitations-and-future-work)
10. [Contributing](#contributing)
11. [License](#license)

### **Introduction**
Monkeypox (MPOX) is an emerging zoonotic disease that has seen a resurgence in human cases globally since 2022. Accurate forecasting of Monkeypox incidence is crucial for public health planning and intervention. This project uses historical case data, explores key epidemiological trends, and applies forecasting techniques to model future cases.

### **Project Objectives**
- **Analyze Historical Data**: To identify key trends and patterns in global Monkeypox cases.
- **Develop Predictive Models**: Using ARIMA and SARIMA models to forecast future case numbers.
- **Visualize Findings**: To present complex data and results in an intuitive format using plots and visualizations.
- **Provide Recommendations**: Based on the forecast results, suggest actionable strategies for public health authorities.

### **Data Sources**
The project utilizes publicly available data from reputable sources:
- **World Health Organization (WHO)**: [Monkeypox Situation Dashboard](https://www.who.int/emergencies/situations/monkeypox-2022)
- **Centers for Disease Control and Prevention (CDC)**: [Monkeypox Cases and Data](https://www.cdc.gov/poxvirus/monkeypox/index.html)
- **Global Health Observatory (GHO)**: [GHO Data Repository](https://www.who.int/data/gho)

### **Methodology**
The project employs a multi-step approach involving:
1. **Data Collection and Preprocessing**: Importing datasets, handling missing values, and normalizing case numbers.
2. **Time Series Analysis**: Using decomposition to identify trend, seasonality, and residual components.
3. **Model Selection and Training**: Implementing ARIMA and SARIMA models to forecast future case trends.
4. **Model Evaluation**: Using metrics like Root Mean Square Error (RMSE) and Mean Absolute Percentage Error (MAPE) to assess model accuracy.
5. **Visualization**: Creating informative plots to present key insights and results.

### **Results and Visualizations**
- **Global Monkeypox Cases and Deaths Over Time**: Visualizing historical trends.
- **Top 10 Locations by Total Cases and Cases per Million**: Identifying regions with the highest burden.
- **Case Fatality Rate Analysis**: Understanding disease severity.
- **Forecasting Plots**: Predictions using ARIMA and SARIMA models, including next-year projections.

### **Project Structure**
The repository is structured as follows:

```
├── data/                      # Directory for datasets (raw and processed)
│   ├── mpox_cases_global.csv
│   └── additional_data_sources/
├── notebooks/                 # Jupyter notebooks for exploratory analysis and model building
│   ├── data_analysis.ipynb
│   └── forecasting_models.ipynb
├── plots/                     # Directory for generated plots and visualizations
│   ├── global_cases_trend.png
│   └── sarima_forecast.png
├── README.md                  # Project description and overview
├── requirements.txt           # Python dependencies and libraries
└── src/                       # Source code for data processing and modeling
    ├── data_preprocessing.py
    ├── arima_model.py
    └── sarima_model.py
```

### **How to Run the Project**
To run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/monkeypox-forecasting.git
   cd monkeypox-forecasting
   ```

2. **Create a Virtual Environment** (Optional):
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   Install the required packages using the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebooks**:
   Open the project’s Jupyter notebooks to run the analysis and model building scripts:
   ```bash
   jupyter notebook notebooks/data_analysis.ipynb
   ```

5. **View Plots and Results**:
   Once the analysis is complete, navigate to the `plots/` directory to view generated visualizations.

### **Dependencies**
The following Python libraries are required for this project:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `scikit-learn`
- `jupyter`

To install them, run:
```bash
pip install -r requirements.txt
```

### **Limitations and Future Work**
While the project offers valuable insights, it has certain limitations:
- **Data Quality**: The accuracy of the models is dependent on the quality and completeness of the underlying data.
- **Model Complexity**: The ARIMA and SARIMA models used may not capture all the nuances of disease spread.
- **Future Enhancements**: Incorporating machine learning models such as LSTM or Prophet could improve predictive accuracy.

### **Contributing**
Contributions are welcome! If you'd like to contribute to this project, please open an issue or submit a pull request. Ensure that your code adheres to the existing style and is well-documented.

### **License**
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
