# Sentiment_Analysis_Project
# Hybrid CNN-LSTM for Sentiment Analysis of Customer Reviews

## Project Description

This project implements a Hybrid CNN-LSTM network for sentiment analysis of customer reviews. It leverages CNNs for feature extraction and LSTMs for sequential understanding. Using pre-trained GloVe embeddings and trained on Amazon reviews, the model achieved a test accuracy of ~89.46% in classifying sentiments.

## Key Features

-   **Hybrid CNN-LSTM Architecture:** Combines Convolutional Neural Networks (CNNs) for local feature extraction and Long Short-Term Memory (LSTMs) networks for understanding sequential dependencies in text.
-   **Sentiment Classification:** Accurately classifies customer reviews as positive or negative.
-   **GloVe Embeddings:** Utilizes pre-trained GloVe word embeddings for rich semantic representations of words.
-   **Amazon Reviews Dataset:** Trained and evaluated on a subset of real-world Amazon customer reviews.
-   **High Performance:** Achieved a test accuracy of approximately 89.46%.

## Dataset

The project uses a subset of Amazon customer reviews. The dataset is structured with labels indicating positive or negative sentiment. The specific files used are `train.txt.txt` and `test.txt.txt`.

## Model Architecture

The model's architecture is a hybrid design:

1.  **Embedding Layer:** Utilizes pre-trained GloVe embeddings to convert words into dense vector representations.
2.  **Convolutional Layers (CNN):** Processes the embedded sequences to extract local features and patterns.
3.  **Long Short-Term Memory (LSTM) Layers:** Captures long-range dependencies and contextual information from the features extracted by the CNN, handling the sequential nature of text.
4.  **Dense Layers:** Fully connected layers for classification, ending with a sigmoid activation for binary sentiment prediction.

## Results

Upon evaluation, the Hybrid CNN-LSTM model demonstrated strong performance:

-   **Test Score (Loss):** 0.2725
-   **Test Accuracy:** 0.8946 (89.46%)

## Setup and Usage

To run this project, you will need the following:

### Dependencies

Install the necessary Python libraries using pip:

```bash
pip install numpy pandas bz2 chardet re tensorflow keras
```

### Data

Ensure that the `glove.twitter.27B.100d.txt`, `train.txt.txt`, and `test.txt.txt` files are available in the specified path:
`/content/drive/MyDrive/Colab Notebooks/Amazon Polarity/
`

### Running the Notebook

1.  **Clone the repository** (if applicable).
2.  **Open the Jupyter/Colab notebook.**
3.  **Run all cells** sequentially. The notebook will perform data loading, preprocessing, model training, and evaluation.

## Developed By

*   **Muhammad Zeeshan Qasim
