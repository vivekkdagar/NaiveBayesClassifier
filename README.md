# Multinomial Naive Bayes Language Classification Tutorial

This repository provides a tutorial on implementing language classification using the Multinomial Naive Bayes algorithm. The tutorial includes a Python implementation to detect the language of a given text. The code consists of two main files: `main.py` for user interaction and `detector.py` containing the `LanguageClassifier` class.

## Overview

The Multinomial Naive Bayes algorithm is widely used for text classification tasks, including language identification. This tutorial demonstrates how to train a language classifier using a provided dataset and then use the trained model to predict the language of input text.

## Prerequisites

Before running the code, ensure you have the following dependencies installed:

- Python
- Required libraries: `requests`, `bs4`, `pandas`, `scikit-learn`, `joblib`

Install the necessary dependencies using the following command:

```bash
pip install requests bs4 pandas scikit-learn joblib
```

## Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/vivekkdagar/language-classification-tutorial.git
   cd language-classification-tutorial
   ```

2. **Run the Main Script:**
   ```bash
   python3 main.py
   ```

3. **Select Data Source and input data:**
   - Choose the mode ('raw', 'file', or 'website') to input text data.

4. **Results:**
   - The predicted language for the provided text will be displayed.

## Code Structure

- `main.py`: Handles user interaction and data input.
- `detector.py`: Contains the `LanguageClassifier` class responsible for training and predicting languages.

## Data Preprocessing

The `LanguageClassifier` class preprocesses the training data by removing special characters and transforming the text into a bag-of-words representation using the `CountVectorizer` from scikit-learn.

## Training the Model

The tutorial uses a provided dataset, "Language Detection.csv," to train the Multinomial Naive Bayes model. The model is then serialized using the `joblib` library for future use.

## Additional Notes

- To modify or extend the training dataset, edit the "Language Detection.csv" file.
- Adjust the HTML tag in the `scrape_website` function within `main.py` based on your specific use case.

## References

- [Language Detection Dataset on Kaggle](https://www.kaggle.com/datasets/basilb2s/language-detection)
- [Beautiful Soup documentation](https://www.crummy.com/software/BeautifulSoup/bs4)
