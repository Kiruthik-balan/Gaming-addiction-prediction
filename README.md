# Gaming Addiction Prediction

This project aims to predict gaming addiction, measured as "Engagement Level", based on various player characteristics and behaviors. The dataset contains information on player demographics, gaming habits, and other factors to classify players into different engagement levels (e.g., High, Low).

## Problem Statement
This project analyzes player behavior in online gaming environments, utilizing variables such as:
- Player age
- Gender
- Location
- Game genre
- Playtime hours
- In-game purchases
- Game difficulty
- Sessions per week
- Average session duration

The goal is to predict the target variable `EngagementLevel`, which serves as a proxy for gaming addiction.

## Dataset
The dataset includes:
- **PlayerID**: Unique identifier for each player.
- **Age**: Player’s age.
- **Gender**: Player's gender.
- **Location**: Player’s geographical region.
- **GameGenre**: Type of games played (e.g., Action, Strategy, Sports).
- **PlayTimeHours**: Total playtime in hours.
- **InGamePurchases**: Binary indicator of whether the player makes in-game purchases.
- **GameDifficulty**: Difficulty level of the games.
- **SessionsPerWeek**: Number of gaming sessions per week.
- **AvgSessionDurationMinutes**: Average duration of each gaming session.
- **AchievementsUnlocked**: Number of achievements unlocked in-game.
- **EngagementLevel**: Target variable indicating the player’s level of engagement (High, Medium, Low).

## Approach

1. **Data Preprocessing**:
    - Importing the dataset.
    - Handling missing values.
    - Encoding categorical variables.
    - Data normalization.

2. **Feature Selection**:
    - Using techniques such as Variance Threshold, Random Forest Classifier, and SelectKBest to select the most relevant features.

3. **Oversampling**:
    - Addressing class imbalance using the SMOTE (Synthetic Minority Over-sampling Technique) method.

4. **Model Training**:
    - Various machine learning algorithms were explored for classification, including RandomForest and others.
    - Evaluating model performance using metrics like accuracy, confusion matrix, and classification report.

## Libraries Used
- **pandas**: Data manipulation and analysis.
- **seaborn**: Data visualization.
- **scikit-learn**: Machine learning algorithms and metrics.
- **imbalanced-learn**: For handling imbalanced datasets.
- **matplotlib**: Plotting and visualizations.

## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/gaming-addiction-prediction.git
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Gaming_addiction_prediction.ipynb
    ```

4. Run the cells sequentially to preprocess the data, train the model, and evaluate the results.

## Results
The model successfully predicts the engagement level of players with high accuracy. Detailed evaluation metrics and visualizations of model performance are available in the notebook.

## Future Work
- Further optimization of feature selection and model hyperparameters.
- Exploration of deep learning models for better prediction accuracy.
