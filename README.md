# Sentiment Analysis with DistilBERT (IMDB Dataset)

This repository demonstrates a **Sentiment Analysis** project leveraging the power of **DistilBERT (uncased)**. The model is fine-tuned on the IMDB movie reviews dataset to classify reviews as either positive or negative.

## Features

- **Model**: Fine-tuned DistilBERT (uncased), a lightweight and efficient variant of BERT.
- **Dataset**: IMDB dataset containing 50,000 movie reviews (balanced between positive and negative sentiments).
- **Libraries Used**: Hugging Face Transformers, PyTorch, and scikit-learn.
- **Pipeline**:
  - Tokenization and text preprocessing using Hugging Face Tokenizer.
  - Fine-tuning the DistilBERT model on the IMDB dataset.

## Installation

To set up the environment, clone the repository and install the required dependencies.

```bash
# Clone the repository
git clone https://github.com/MahnoorMali-k/SentimentAnalysis.git

# Navigate to the project directory
cd SentimentAnalysis

# Install dependencies
pip install -r requirements.txt
```

## Dataset

The IMDB dataset is available through the `datasets` library from Hugging Face. It includes 25,000 labeled training examples and 25,000 labeled testing examples.

## How It Works

1. **Data Loading and Preprocessing**:
   - The IMDB dataset is loaded using the `datasets` library.
   - Reviews are tokenized using DistilBERT's tokenizer.

2. **Model Fine-tuning**:
   - DistilBERT is fine-tuned on the training set using PyTorch and the Hugging Face Trainer API.
   - Training is optimized using AdamW optimizer and a linear learning rate scheduler.

3. **Evaluation**:
   - The model is evaluated on the test set.

## Quick Start

You can open the provided Colab notebook and run all cells to perform training and evaluation on a GPU:

[Open in Google Colab](https://colab.research.google.com/)

## Project Structure

```plaintext
SentimentAnalysis-DistilBERT/
├── SentimentAnalysis.ipynb # Colab notebook for training and evaluation
├── requirements.txt        # Dependencies
├── README.md               # Project documentation
```

## Dependencies

The following libraries are required to run the project:

- Transformers
- Datasets
- PyTorch
- scikit-learn

Install them using:

```bash
pip install transformers datasets torch scikit-learn
```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Hugging Face Transformers](https://huggingface.co/docs/transformers/)
- [IMDB Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)

---

Happy analyzing! 🚀
