Dataset Overview

The dataset used in this project contains information about vehicles, including their brand, model, year of registration, price in euros, power specifications, transmission type, fuel type, fuel consumption, mileage, and offer description.
Dataset Cleaning and Preprocessing

The dataset underwent several cleaning and preprocessing steps to prepare it for machine learning tasks:

    Cleaning 'year' Column:
        Invalid year entries were filtered out using a function that converts valid years between 1995 and 2023, dropping rows with NaN values afterward.

    Converting Data Types:
        The 'year' column was converted to integers.
        Several numeric columns ('price_in_euro', 'power_kw', 'power_ps', 'fuel_consumption_l_100km', 'mileage_in_km') were converted to numeric types using a function that handles errors gracefully.

    Handling Missing Values:
        Missing numeric values were imputed using the median value strategy.
        Categorical missing values were imputed using the most frequent value strategy.

    Scaling and Encoding:
        Numeric features were standardized using StandardScaler.
        Categorical features were encoded using OneHotEncoder, with unknown categories ignored.

    Outlier Handling:
        Outliers in numeric columns were replaced with median values to improve model robustness.

Machine Learning Pipeline

The preprocessing steps described above were integrated into a machine learning pipeline using Pipeline and ColumnTransformer from scikit-learn. The pipeline prepares the data for training and testing machine learning models.
