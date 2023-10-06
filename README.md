# News Classification with Logistic Regression

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Data Preprocessing](#data-preprocessing)
- [Text Stemming](#text-stemming)
- [Text Vectorization](#text-vectorization)
- [Splitting the Dataset](#splitting-the-dataset)
- [Training the Model](#training-the-model)
- [Evaluation](#evaluation)
- [Making Predictions](#making-predictions)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This code is designed for classifying news articles as either real or fake news using a logistic regression model. It preprocesses the data, applies text stemming, converts text into numerical features using TF-IDF, and trains a logistic regression model for classification.

## Dataset
The dataset used for this project contains news articles with the following columns:
- `id`: Unique identifier for each news article.
- `title`: The title of the news article.
- `author`: The author of the news article.
- `text`: The text of the article (may be incomplete).
- `label`: A label marking whether the news article is real (0) or fake (1) news.

## Dependencies
Before running the code, make sure you have the following dependencies installed:
- NumPy
- Pandas
- NLTK
- Scikit-Learn

You can install the required NLTK data by running `nltk.download('stopwords')`.

## Usage
1. Clone this repository to your local machine.
2. Ensure you have the required dependencies installed.
3. Modify the data file path in the code if your dataset is located in a different location.
4. Run the code using a Python interpreter.

## Data Preprocessing
- Missing values are replaced with empty strings.
- Author names and news titles are merged into a new 'content' column.

## Text Stemming
Text stemming is applied to reduce words to their root forms using the NLTK Porter Stemmer. This helps in dimensionality reduction.

## Text Vectorization
The textual data is converted into numerical data using TF-IDF vectorization, representing word importance in the corpus.

## Splitting the Dataset
The dataset is split into training and testing sets using `train_test_split`.

## Training the Model
A logistic regression model is trained using the training data.

## Evaluation
- The accuracy score is calculated on both the training and test datasets to assess model performance.

## Making Predictions
You can use the trained model to make predictions on new data. Provide the text data in the same format and use the model's `predict` function.

## Contributing
Contributions are welcome! Please fork this repository and submit pull requests to suggest improvements or fix issues.

## License
This code is available under the [MIT License](LICENSE).
