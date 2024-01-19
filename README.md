# CS210_Project
CS210 Data Analysis Project
Spotify Listening Habits Analysis

Project Overview

This project aims to analyze and predict Spotify listening habits based on historical streaming data. The core hypothesis is that there are significant differences in genre preferences across different times of the day. A machine learning model was developed to forecast future listening minutes for various genres and timeframes, providing insights into the user's music listening patterns.

Repository Structure

This repository contains the following files and folders:

Data_With_Genres.json: The preprocessed dataset with genres and listening times.
model/: Directory containing the trained machine learning model and its serialization.
notebooks/: Colab notebooks with the analysis, model training, and prediction steps.
requirements.txt: A text file listing the dependencies required to run the project.
README.md: Documentation providing an overview and instructions for the project.
Hypothesis

The working hypothesis is that the user's preference for the 'compositional ambient' genre is higher during midnight (00:00 to 06:00) and morning (06:00 to 12:00) hours compared to other times of the day.

Data Collection

The dataset is composed of Spotify streaming history, which includes timestamps, genres listened to, and the duration of each listening session.

Data Preprocessing

The streaming data was cleaned and preprocessed to ensure quality and consistency. This process involved handling missing values, exploding nested genre lists into separate records, and creating time-related features for analysis.

Exploratory Data Analysis (EDA)

Preliminary EDA was performed to understand the data's structure and distribution. This included generating a heatmap of the top 10 genres by listening counts across different hours of the day.

Feature Engineering

Features relevant to the hypothesis were crafted, such as distinguishing between weekend and weekday listening sessions to capture potential behavioral differences.

Model Selection and Development

A RandomForestRegressor model was selected due to its robustness and ability to model complex patterns. The model underwent hyperparameter tuning to enhance its predictive performance.

Future Predictions

The trained model was used to make predictions about future listening minutes based on the hour, day of the week, and genre.

Instructions for Running the Project

To run the project, follow these steps:

Ensure Python 3.8+ is installed on your system.
Clone the repository to your local machine.
Install the required dependencies using pip install -r requirements.txt.
Navigate to the notebooks/ directory and open the Jupyter notebooks to view the analysis and predictions.
Contributing

Contributions to this project are welcome. Please open an issue to discuss proposed changes or submit a pull request.

License

This project is open-sourced under the MIT License. See the LICENSE file for more details.

Contact

For any further questions or feedback, please contact the repository owner.
