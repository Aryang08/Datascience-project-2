# Real-Time Stock Price Dashboard Web App

## Overview

This project demonstrates how to build an interactive web application for visualizing real-time stock prices using the Mercury framework. The application leverages several Python libraries to fetch, analyze, and visualize stock data.

## Objectives

By the end of this project, you will be able to:

- Utilize Python libraries for financial data analysis, including `yfinance` and `cufflinks`.
- Create interactive visualizations to gain insights into stock performance and portfolio management.
- Calculate and visualize cumulative returns for a weighted portfolio of multiple stocks in the semiconductor industry.
- Deploy the application using the Mercury framework, allowing for easy sharing of your stock data analysis with a global audience.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Setup Instructions](#setup-instructions)
4. [Usage](#usage)
5. [Deployment](#deployment)
6. [Acknowledgements](#acknowledgements)

## Prerequisites

- Python 3.x
- Jupyter Notebook
- Internet connection for downloading stock data

## Installation

Install the required libraries using the following command:

```bash
pip install yfinance ipyvuetify cufflinks mercuryA

## Usage

1. Launch the Jupyter Notebook and run the cells sequentially.
2. Interact with the widgets to select the stock ticker and the time period for analysis.
3. Visualizations will update based on your selections.

## Deployment

To deploy the application using Mercury: 
->my dashboard:{https://firstdeploy.runmercury.com/app/stockprizeviz}

1. Sign up for a free account at [Mercury](https://mercury.dev).
2. Log in and create a new site.
3. Upload your Jupyter Notebook and `requirements.txt`.
4. Open the site to access your web app.

## Acknowledgements

- **Mercury Framework**: An open-source framework for building web apps from Jupyter Notebooks.
- **yfinance**: Library for downloading financial data from Yahoo Finance.
- **Cufflinks**: Simplifies data visualization with Plotly for Pandas DataFrames.
