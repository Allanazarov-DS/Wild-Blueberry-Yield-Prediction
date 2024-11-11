# Wild Blueberry Yield Prediction

This project aims to predict the yield of wild blueberries using various environmental and pollination-related factors. The dataset includes features related to temperature ranges, bee activity, rain frequency, and fruit characteristics, with `yield` as the target variable.

## Project Overview

The objective of this project is to build a regression model to accurately predict blueberry yield, leveraging features like pollinator activity and temperature metrics.

## Dataset

The dataset consists of the following key columns:

| **Column Name**           | **Description**                                                                                                                                 |
|---------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| **Clone Size**            | Size of the plant clone, impacting yield.                                                                                                       |
| **Honeybee Activity**     | Activity level or count of honeybees, important for pollination.                                                                                |
| **Bumblebee Activity**    | Activity level of bumblebees, influencing pollination and fruit development.                                                                    |
| **Andrena Bee Activity**  | Activity level of Andrena bees, solitary pollinators contributing to pollination.                                                              |
| **Osmia Bee Activity**    | Activity level of Osmia bees, another solitary pollinator species.                                                                             |
| **Max Upper Temperature** | Maximum temperature in the upper range, affecting growth and pollination.                                                                      |
| **Min Upper Temperature** | Minimum temperature in the upper range, impacting pollinator behavior.                                                                         |
| **Avg Upper Temperature** | Average temperature in the upper range, showing typical pollination and growth conditions.                                                     |
| **Max Lower Temperature** | Maximum temperature in the lower range, influencing health during cooler periods.                                                              |
| **Min Lower Temperature** | Minimum temperature in the lower range, with implications for frost risk.                                                                      |
| **Avg Lower Temperature** | Average temperature in the lower range, impacting plant and pollinator activity.                                                               |
| **Rainy Days**            | Total rainy days, affecting pollinator activity and yield.                                                                                     |
| **Avg Rainy Days**        | Average rainy days over a period, influencing pollination and plant health.                                                                    |
| **Fruit Set**             | Percentage or count of flowers turning into fruit, indicating pollination effectiveness.                                                       |
| **Fruit Mass**            | Average mass of individual fruits, directly impacting yield.                                                                                   |
| **Seed Count**            | Number of seeds per fruit, reflecting pollination success.                                                                                     |
| **Yield** (Target)        | Total agricultural output per unit area, the target variable.                                                                                  |

## Project Workflow

1. **Data Preprocessing**:
   - Dropped non-essential columns.
   - Scaled features using different scaling techniques (e.g., StandardScaler, RobustScaler).
   - Engineered features to improve model performance.

2. **Model Training**:
   - Implemented regression models such as RandomForestRegressor and LinearRegression.
   - Evaluated models using metrics like Mean Absolute Error (MAE) and R² Score.

3. **Evaluation**:
   - Tested models on validation data.
   - Selected the model with the best performance for yield prediction.

## Getting Started

1. Clone this repository:

   ```bash
   git clone git@github.com:Allanazarov-DS/Wild-Blueberry-Yield-Prediction.git
   ```

2. Install the necessary packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the analysis notebook to see the model training and evaluation steps:

   ```bash
   jupyter notebook analysis.ipynb
   ```

## Results

The final model's performance is evaluated on mean absolute error and R² score to determine the most effective model for predicting yield.

## Contributing

Feel free to submit issues or pull requests if you would like to contribute to this project.

## License

This project is licensed under the MIT License.
