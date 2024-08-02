# Twitter Sentiment Analysis Project

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Table of Contents

- [Project Overview](#project-overview)
- [Motivation](#motivation)
- [Dataset](#dataset)
- [Project Highlights](#project-highlights)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

The **Twitter Sentiment Analysis Project** aims to detect hate speech in tweets. Specifically, it classifies tweets as containing hate speech (racist/sexist) or not. The task is to distinguish between tweets with hate speech (label '1') and those without (label '0') using a dataset of 31,962 labeled tweets.

## Motivation

With the Paris Olympics 2024 and the US elections (Trump vs. Kamala) generating a high volume of tweets, there's a growing need to address and mitigate negativity on social media. This project is designed to help spread positivity and reduce the impact of hate speech in online conversations.

## Dataset

The dataset consists of 31,962 labeled tweets, where each entry includes:
- **Tweet ID**
- **Label**: 
  - `1` for racist/sexist tweets
  - `0` for non-racist/non-sexist tweets
- **Tweet Text**

## Project Highlights

- **Data Preprocessing**: Cleaned and prepared tweet text to remove noise and irrelevant content.
- **Feature Extraction**: Employed `TfidfVectorizer` to convert text data into numerical features.
- **Model Training**: Utilized Logistic Regression to classify tweets.
- **Visualization**:
  - Word clouds for positive and negative words.
  - Bar graphs for the top 10 most frequently used positive and negative words.
- **Evaluation**: Achieved a model accuracy of 95.00%.

## Installation

To get started with the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/twitter-sentiment-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd twitter-sentiment-analysis
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Data Preprocessing**:
    ```python
    from preprocessing import preprocess_data
    data = preprocess_data('path/to/dataset.csv')
    ```
2. **Feature Extraction**:
    ```python
    from feature_extraction import extract_features
    features = extract_features(data)
    ```
3. **Model Training**:
    ```python
    from model_training import train_model
    model = train_model(features, labels)
    ```
4. **Model Evaluation**:
    ```python
    from model_evaluation import evaluate_model
    evaluate_model(model, test_data, test_labels)
    ```
5. **Visualization**:
    ```python
    from visualization import create_word_clouds, plot_top_words
    create_word_clouds(data)
    plot_top_words(data)
    ```

## Results

- **Best Model Accuracy**: 95.00%
- **Visualizations**:
  - Word clouds showcasing positive and negative words.
  - Bar graphs illustrating the top 10 most used positive and negative words.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



