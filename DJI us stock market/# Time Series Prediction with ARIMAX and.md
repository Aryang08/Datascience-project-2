# Time Series Prediction with ARIMAX and Random Forest

This project focuses on predicting time series data using ARIMAX (AutoRegressive Integrated Moving Average with eXogenous variables) and Random Forest regression models. The datasets utilized include weather-related data from Laguardia and historical stock market data from the Dow Jones Industrial Average. The project is developed and deployed on the Mercury notebook site.

## Table of Contents

- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Key Functions](#key-functions)
- [Model Evaluation](#model-evaluation)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Features

- **ARIMAX Model**: For time series forecasting with external variables.
- **Random Forest Regression**: For non-linear predictions based on multiple input features.
- **Statistical Tests**: Includes Augmented Dickey-Fuller (ADF) and KPSS tests for stationarity checks.
- **Data Visualization**: Utilizes Matplotlib and Seaborn for exploratory data analysis and result interpretation.
- **Automated Data Download**: Fetches datasets directly from Skills Network.

## Dataset

The project uses two primary datasets downloaded from Skills Network:

1. **Laguardia Weather Data**:
   - **Description**: Contains historical weather data relevant to the prediction model.
   - **Download Link**: 
     ```python
     await skillsnetwork.download_dataset(
         'https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0K1YEN/laguardia.csv'
     )
     laguardia = pd.read_csv('laguardia.csv', dtype='str')
     ```

2. **Dow Jones Industrial Average**:
   - **Description**: Historical stock market data for forecasting stock prices.
   - **Download Link**: 
     ```python
     await skillsnetwork.download_dataset(
         'https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0K1YEN/dow_jones.csv'
     )
     dow = pd.read_csv('dow_jones.csv', dtype='str')
     ```

## Installation

### Prerequisites

- **Python 3.8 or higher**: Ensure you have Python installed. You can download it from [here](https://www.python.org/downloads/).

### Clone the Repository

```bash
git clone https://github.com/Aryang08/Data-science-Learning-project.git
cd Data-science-Learning-project
Create a Virtual Environment (Optional but Recommended)
bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies
Ensure you have pip installed. Then, install the required Python packages using the requirements.txt file:

bash
Copy code
pip install -r requirements.txt
Project Structure
bash
Copy code
your-repo-name/
│
├── notebook.ipynb          # Main Jupyter notebook for analysis and modeling
├── requirements.txt        # Python dependencies
├── README.md                # Project documentation
└── LICENSE  
Congratulations! You have completed the lab
Authors
Wojciech "Victor" Fulmyk is a Data Scientist at IBM and a PhD candidate at the University of Calgary

Other Contributors
Sina Nazeri is a Data Scientist at IBM and a PhD candidate at Simon Fraser University in Vancouver