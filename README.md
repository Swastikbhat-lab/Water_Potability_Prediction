

#  Water Potability Prediction

This project aims to predict the potability of drinking water using various water quality metrics. The dataset used includes multiple features that assess water quality, such as pH level, hardness, solids, chloramines, sulfate, conductivity, organic carbon, trihalomethanes, and turbidity.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)


## Introduction

Ensuring the safety of drinking water is crucial for public health. This project uses machine learning techniques to classify water samples as potable or non-potable based on their characteristics. The goal is to provide an automated system that can aid in water quality monitoring and decision-making.

## Dataset

The dataset used in this project contains various water quality parameters:
- pH value
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- Organic carbon
- Trihalomethanes
- Turbidity
- Portability (target variable)

## Features

- **pH**: pH value of water (0 to 14).
- **Hardness**: Capacity of water to precipitate soap in mg/L.
- **Solids**: Total dissolved solids in ppm.
- **Chloramines**: Amount of Chloramines in ppm.
- **Sulfate**: Amount of Sulfates dissolved in mg/L.
- **Conductivity**: Electrical conductivity of water in μS/cm.
- **Organic carbon**: Amount of organic carbon in ppm.
- **Trihalomethanes**: Concentration of trihalomethanes in μg/L.
- **Turbidity**: Measure of light emittance in NTU.
- **Potability**: Indicates if water is safe for human consumption (1: Potable, 0: Not potable).

## Installation

To run this project, you need to have Python installed on your system. It is recommended to use a virtual environment to manage dependencies. Follow the steps below to set up the project:

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/drinking-water-potability-prediction.git
    cd drinking-water-potability-prediction
    ```

2. Create a virtual environment and activate it:
    ```sh
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Ensure you have Jupyter Notebook installed. If not, you can install it using:
    ```sh
    pip install notebook
    ```

2. Open the Jupyter Notebook:
    ```sh
    jupyter notebook
    ```

3. Open the `Drinking_Water_Potability_Prediction.ipynb` file in Jupyter Notebook and run the cells to see the analysis and results.

## Results

The notebook includes data exploration, preprocessing, model training, and evaluation steps. Various machine learning models are used to predict water potability, and their performance is compared based on accuracy and other metrics.


