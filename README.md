Non-Verbal Tourist Data Analysis and Augmentation
Description
This project explores a dataset focusing on non-verbal communication attributes of tourists. It uses data analysis, augmentation, and machine learning techniques to understand and predict customer types based on attributes like gestures, audio cues, and proxemics.

The notebook is divided into the following sections:

1. Data Loading and Preprocessing
Loads the dataset using pandas.
Handles missing values (? replaced or addressed).
Maps categorical values (e.g., like, dislike, indifferent) to numerical representations (-1, 0, 1).
Ensures all columns are properly typed for further analysis.
2. Exploratory Data Analysis (EDA)
Summarizes key statistics of numerical and categorical variables.
Visualizes distributions and relationships between features.
Highlights patterns in non-verbal attributes like proxemics, gestures, and emotional climate.
3. Feature Engineering
Extracts relevant features for analysis and modeling.
Creates new features based on existing attributes (e.g., aggregating gesture preferences).
Encodes categorical variables for machine learning compatibility.
4. Data Augmentation
Introduces synthetic data creation to enhance the dataset's diversity:
Adds noise to numerical features like Tense - relaxed and Hostile - friendly.
Shuffles categorical features within columns to create new combinations.
Saves the augmented dataset for additional analysis and modeling.
5. Modeling and Machine Learning
Trains a Random Forest classifier to predict the Type of Client (target variable).
Evaluates the model using metrics such as accuracy, precision, and recall.
Hyperparameter tuning to optimize the Random Forest model.
6. Results and Insights
Presents the key findings from the analysis and model predictions.
Discusses potential applications of the model in understanding tourist behavior.
Dataset Description
Attributes:
Demographic Information:

sex: Gender of the tourist (M/F).
age: Age of the tourist.
country: Country of origin.
returning: Whether the tourist is a returning visitor.
Non-Verbal Communication Features:

GImg1, GImg2, GImg3, PImg1 to PImg5: Preferences for different gestures and postures.
Tense - relaxed: Numerical scale for emotional state.
Authoritative - anarchic, Hostile - friendly: Scales for emotional climate.
Audio Cues:

TAudio1 to TAudio3, QAudio1 to QAudio3: Preferences for audio cues.
Proxemics:

Preferred physical distance between the tourist and others.
Target Variable:

Type of Client: Encoded type of tourist (e.g., 0, 1, or 2).
