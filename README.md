# Anime_dataset_EDA
This project builds a regression model to predict the number of favorites an anime character receives, using structured and text data. It combines data cleaning, feature engineering, visualization, and machine learning, and demonstrates core skills relevant to Data Analytics (DA), Data Engineering (DE), Analytics Engineering (AE), and Business Intelligence (BI) roles.

📦 Dataset
Source: Kaggle: Anime Character Database (July 2025)

Rows: 202,984 characters

Columns: 10 fields including name, favorites, about, nicknames, image_url, etc.

🔧 Cleaning & Preprocessing
The raw dataset includes missing values and mixed data types. The following steps were taken:

Removed HTML tags from the about column.

Parsed the nicknames field into countable lists.

Engineered features like name_length, has_kanji, has_about, and nickname_count.

🎯 Target Variable
favorites – the number of times a character is marked as favorite by MyAnimeList users.
This is a regression task to predict this continuous numeric value.

✅ Features Used
Feature	Description
name_length	Character name length
has_kanji	Whether kanji name is present
has_about	Whether a character has an 'about' bio
nickname_count	Number of nicknames
about (optional)	Character description (used with NLP)

📈 Models Trained
Linear Regression

Random Forest Regressor

Random Forest with TF-IDF vectorization on about text

📊 Evaluation Metrics
RMSE (Root Mean Squared Error)

R² Score
