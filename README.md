# Diamond Price Prediction

This project aims to predict the price of diamonds based on various features such as size, depth, color, and clarity. The goal of this project is to use the **Linear Regression** algorithm to predict diamond prices based on available data.

## Data

The data consists of two CSV files:

1. **diamonds_train.csv**: Training dataset for training the model.
2. **diamonds_test.csv**: Testing dataset for evaluating the model.

The features in the data include:

- **cut**: Diamond cut (Fair, Good, Very Good, Premium, Ideal)
- **color**: Diamond color (J, I, H, G, F, E, D)
- **clarity**: Diamond clarity (I1, SI2, SI1, VS2, VS1, VVS2, VVS1, IF)
- **x, y, z**: Diamond dimensions (length, width, depth)
- **depth**: Depth of the diamond
- **table**: Top surface area of the diamond
- **price**: Price of the diamond (target variable)

## Installation and Setup

To use this project, you need to install the following libraries:

```bash
pip install numpy pandas scikit-learn
```

## Data Preprocessing Steps

1. **Data Processing**:
   - Categorical features like **cut**, **color**, and **clarity** were encoded into numerical values using **Label Encoding**.
   - The **IQR method** was used to remove outliers in the `x` and `y` features.

2. **Scaling Data**:
   - **MinMaxScaler** was used to scale numerical features (`x`, `y`, `z`, `depth`, `table`) to ensure the model works correctly.

3. **Train-Test Split**:
   - The dataset was split into training and testing sets to allow the model to train and then be evaluated.

## Model

- **Linear Regression** was used for modeling the data.
- The model was trained using the training data and then evaluated using the testing data.

## Results

The model's performance was evaluated using the **R-squared (r²)** metric, which indicates the model's quality.

```python
accuracy = r2_score(y_test, y_predict)
print(accuracy)
```

## Usage

To use the model, you can input new data and predict diamond prices. You can also modify the code to improve the model or experiment with other algorithms.

## Files

- **diamonds_train.csv**: Training data
- **diamonds_test.csv**: Test data
- **diamond_price_prediction.ipynb**: Project code

## Collaboration

If you would like to collaborate on this project or have suggestions for improvements, feel free to share your feedback with us.

---

This English version of the README should be ready to go on GitHub! Let me know if you need any further tweaks.
