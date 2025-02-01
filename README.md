# NEET Rank Prediction and Quiz Analysis

## Project Overview

This project focuses on analyzing student performance through quiz data and predicting NEET (National Eligibility cum Entrance Test) ranks based on quiz performance metrics. The project includes various stages of data exploration, feature engineering, model training, and result visualization.

The primary objective is to:
1. Analyze quiz data to understand student performance across different topics.
2. Train a model to predict NEET ranks based on quiz performance features.
3. Provide predictions on possible college placements based on the predicted rank.
4. Visualize the average performance across topics to gain insights into areas of strength and weakness.

## Approach Description

The approach for the project is divided into several phases:
1. **Data Collection**: The project fetches data from various online sources:
   - Quiz data (questions and answers)
   - Quiz submission data (student responses)
   - Historical quiz performance data (student scores and other metrics)

2. **Data Cleaning**: Once the data is fetched, the project ensures that the data is valid and properly formatted. It handles missing or incomplete data by checking if the required fields are present.

3. **Data Analysis**: The analysis involves computing the average performance for each topic in the quiz. Additionally, feature engineering is applied to calculate metrics like `avg_score` and `accuracy` based on individual student performance.

4. **Model Training**: A Random Forest Regressor model is trained on the historical data, using features like `avg_score` and `accuracy` to predict the student’s NEET rank.

5. **Prediction and College Suggestion**: After training the model, the project uses it to predict the NEET rank for a given student, and suggests a suitable college based on the rank.

6. **Visualization**: The project visualizes the average performance per topic using a bar chart, providing insights into areas that need improvement.

## Setup Instructions

### Prerequisites

Before running the project, ensure you have the following installed:
- Python (>= 3.7)
- `pip` (Python package manager)



   ```bash
   git clone https://github.com/yourusername/neet-rank-prediction.git
   cd neet-rank-prediction
