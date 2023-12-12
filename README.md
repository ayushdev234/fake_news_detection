# Fake News Detection Project

## Objective

The objective of this project is to build a fake news detection system using machine learning techniques. The model is trained on a dataset of news articles to distinguish between real and fake news based on their content.

## Libraries Imported

- `numpy` for numerical operations
- `pandas` for data manipulation and analysis
- `re` for regular expressions
- `nltk` for natural language processing tasks
- `sklearn` for machine learning tools and utilities

## Procedure

1. **Dataset Loading:**
   - The news dataset is loaded into a pandas DataFrame from a CSV file (`train.csv`).

2. **Data Preprocessing:**
   - Null values in the dataset are replaced with empty strings.
   - Author names and news titles are merged into a single column called 'content'.
   - Text data is preprocessed using stemming and removing stopwords from NLTK.

3. **Feature Extraction:**
   - TF-IDF Vectorizer is used to convert the text data into numerical features.

4. **Data Splitting:**
   - The dataset is split into training and testing sets using `train_test_split`.

5. **Model Training:**
   - Logistic Regression is chosen as the classification model.

6. **Model Evaluation:**
   - Training data accuracy is calculated using `accuracy_score`.
   - Testing data accuracy is calculated and printed.

7. **Prediction:**
   - A sample news article from the test set is taken for prediction.
   - The model predicts whether the news is real or fake and prints the result.

## Algorithm Steps

1. Load the dataset.
2. Handle missing values.
3. Merge author names and news titles.
4. Apply stemming and remove stopwords using NLTK.
5. Split the dataset into features (X) and labels (Y).
6. Split the data into training and testing sets.
7. Initialize the Logistic Regression model.
8. Train the model on the training data.
9. Evaluate the model on training and testing data.
10. Make predictions on a sample news article.

## Usage of NLTK Library and Stemming

The NLTK library is used for natural language processing tasks. The Porter Stemmer from NLTK is applied to reduce words to their root form, which helps in simplifying the text data and improving model performance.

## Note

Make sure to download the NLTK stopwords dataset using `nltk.download('stopwords')` before running the code.

Feel free to customize the code and experiment with different models and preprocessing techniques.

