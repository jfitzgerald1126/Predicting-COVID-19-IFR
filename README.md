# Modelling COVID-19 Infection Fatality Rate Based On Percentage Of Population Vaccinated Using Linear Regression

The project aims to model the relationship between the COVID-19 Infection Fatality Rate (IFR) and the Percentage of Population Vaccinated (%PV) using linear regression. The project explores how vaccination rates in different countries may impact their infection fatality rates. By creating regression models based on real-world data, the project seeks to gain insights into the potential effects of vaccination on reducing COVID-19 mortality.

## Overview
The project utilizes Python and several Python libraries, such as "matplotlib" and "numpy," to analyze COVID-19 data for selected countries. It consists of three main components:

1. Data Filtering: The "data_filtering.py" file reads COVID-19 data from the "condensed_data.csv" file, filters it based on the chosen country, and converts it into a Python class called "Country." The "Country" class represents a country with related COVID-19 data, such as new deaths per million people, the percentage of the population fully vaccinated per hundred, and the reproduction rate.

2. Data Computations: The "data_computations.py" file computes the data from the "Country" object and forms the regression model. It includes a function to optimize the base mathematical function used to model the relationship between IFR and %PV with SciPy curve fitting. The "Model" class in this file creates a regression model of a country's IFR based on its percentage of the population vaccinated.

3. Data Visualization: The "data_visualization.py" file handles the visualization of the data and models from the "Model" class in an interactive manner. The "Plot" class visualizes the data using the "matplotlib" library and provides an interactive window where the user can toggle the visibility of plots for different countries. This interactive visualization helps users understand the correlation between vaccination rates and infection fatality rates for selected countries.

## How to Use the Project
1. Clone this repository to your local machine.
2. Ensure you have Python and the required libraries installed (e.g., "matplotlib" and "numpy").
3. Make sure the "condensed_data.csv" file is present in the project directory.
4. Customize the countries you want to model by changing the Country input strings in the "main.py" file (e.g., Country('Germany', csv_location)).
5. Run "main.py" to see the interactive visualization of the regression models for the selected countries.

## Inspiration
The project takes inspiration from the COVID-19 Data Explorer by Our World in Data (https://ourworldindata.org/explorers/coronavirus-data-explorer). The goal is to provide similar interactive visualizations for modelling the IFR based on the percentage of the population vaccinated.

