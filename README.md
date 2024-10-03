
# Correlation Analysis and Linear Regression Modeling of Possum Data

This project demonstrates how to conduct correlation analysis and build a linear regression model using a possum dataset. The goal is to explore relationships between numerical features and use linear regression to predict total length (`totlngth`) of a possum based on head length (`hdlngth`) and tail length (`taill`).

## Project Structure
- `possum.csv`: The dataset containing measurements of possums.
- `possum_analysis.py`: The main Python script that performs the correlation analysis and builds a linear regression model.
- `README.md`: Project overview and instructions.
  
## Dataset Overview
The dataset includes various measurements related to possums, such as:
- `hdlngth`: Head length
- `skullw`: Skull width
- `totlngth`: Total length
- `taill`: Tail length
- `footlgth`: Foot length
- `earconch`: Ear length
- `eye`: Eye diameter
- `sex`: Sex of the possum
- `Pop`: Population (categorical)

For this project, we focus on `hdlngth`, `taill`, and `totlngth`.

## Steps in the Analysis
1. **Correlation Analysis**:
   - Analyze the relationship between numerical features using a correlation matrix and heatmap visualization.
   - Understand which features have the strongest correlations.

2. **Linear Regression**:
   - Build a linear regression model to predict `totlngth` (total length) based on the `hdlngth` (head length) and `taill` (tail length).
   - Evaluate the model's performance using metrics such as Mean Squared Error (MSE) and R-squared (R²).
   - Visualize the predicted vs actual values, and analyze residuals.

## Prerequisites

Before running the code, ensure you have Python 3.x and the following libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run

1. Clone the repository or download the files.
2. Ensure the dataset (`possum.csv`) is in the correct directory.
3. Open a terminal and run the script:
   ```bash
   python possum_analysis.py
   ```

4. The script will:
   - Output a correlation matrix and show the heatmap.
   - Train a linear regression model.
   - Output model evaluation metrics like MSE and R².
   - Display visualizations for actual vs predicted values and residuals.

## Outputs

- **Correlation Matrix**: A matrix that displays the correlation coefficients between numeric features.
- **Regression Coefficients**: The coefficients of the linear regression model.
- **Model Evaluation**:
  - **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.
  - **R-squared (R²)**: Explains how well the regression model fits the data.
  
- **Plots**:
  - **Correlation Heatmap**: A visual representation of the correlation matrix.
  - **Actual vs Predicted Values Plot**: Compares predicted total length against actual values.
  - **Residuals Plot**: Shows errors between predicted and actual values.

## Example Results

- **R² score**: A value between 0 and 1 that indicates the strength of the model fit. Closer to 1 is better.
- **MSE**: A lower value indicates better performance of the regression model.

