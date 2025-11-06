☀️ Solar Energy Potential Analysis using K-Means Clustering

Status

Language

License

✅ Completed

Python

MIT

💡 Project Overview

This project implements a data mining methodology to evaluate the potential for renewable (specifically solar) energy generation by analyzing monthly weather patterns. Using K-Means Clustering, we segment months based on their mean maximum and minimum temperatures to identify distinct clusters representing High Solar Potential periods.

The methodology is inspired by the research paper: "Renewable Energy Evaluation using Data Mining Techniques".

🎯 Objective

The primary goal of this notebook is to replicate the data mining approach from the referenced research to:

Analyze a dataset of monthly temperature averages across different cities.

Apply K-Means Clustering to segment the data into optimal groups.

Identify the cluster corresponding to the highest temperatures, which directly correlates with the highest potential for solar radiation and energy output.

⚙️ Methodology

The core of the analysis uses the unsupervised K-Means algorithm (with $k=2$ clusters) on two key features:

Max_Mean_Temp_C (Maximum Mean Temperature in Celsius)

Min_Mean_Temp_C (Minimum Mean Temperature in Celsius)

This simple, yet effective, clustering helps group the 12 calendar months into two distinct climate profiles: Moderate Temperature and High Temperature/High Potential.

📊 Key Results

The model successfully classified the data, yielding two distinct clusters:

Cluster

Description

Representative Months (High Potential Cluster)

Cluster 1

☀️ High Solar Potential

Apr, May, Jun, Jul, Aug, Sep

Cluster 0

Moderate Temperature

Jan, Feb, Mar, Oct, Nov, Dec

This confirms that the clustered months align with the peak summer and pre-monsoon periods, which are generally considered optimal for solar power generation.

<details>
<summary>Click to view raw clustering output</summary>

Cluster 1: High Temperature / High Solar Potential Months 
       City Month  Max_Mean_Temp_C
8   Chennai   Sep             34.0
7   Chennai   Aug             34.4
32  Madurai   Sep             34.4
6   Chennai   Jul             35.0
3   Chennai   Apr             35.1
31  Madurai   Aug             35.3
26  Madurai   Mar             35.8
30  Madurai   Jul             35.9
29  Madurai   Jun             36.8
5   Chennai   Jun             36.9
4   Chennai   May             37.1
27  Madurai   Apr             37.2
28  Madurai   May             37.7


</details>

💻 How to Run the Analysis

Prerequisites

You need Python 3.x installed. The required libraries are listed below.

1. Installation

Clone the repository and install dependencies:

# Clone the repository (replace <Your_Repo_URL> with the actual URL)
git clone (https://github.com/mrdivyanshsk/Data-mining-project)
cd Data-mining-project

# Install required Python libraries
pip install pandas scikit-learn plotly


2. Run the Notebook

The analysis is contained entirely within the Jupyter Notebook.

Jupyter Lab/Notebook:

jupyter notebook sp_pandey_ds01.ipynb


Google Colab:
Alternatively, you can upload the sp_pandey_ds01.ipynb file directly to Google Colab and run the cells sequentially.

📦 Dependencies

Package

Version (Recommended)

Purpose

pandas

>= 2.0.0

Data manipulation and analysis

scikit-learn

>= 1.3.0

K-Means Clustering implementation

plotly

>= 5.14.0

Interactive data visualization (scatter plot)

📝 Data Source

The dataset used in this analysis is synthetic, augmented with the help of an LLM, and contains average monthly temperature data for three Indian cities: Chennai, Kanyakumari, and Madurai.

Features:

City: Location

Month: Calendar month

Max_Mean_Temp_C: Maximum average temperature for the month (°C)

Min_Mean_Temp_C: Minimum average temperature for the month (°C)
