# classificazione_frasi_con_BERT_transformers

A simple sentence classification project using BERT and the Hugging Face Transformers library.

This project was created as a personal exercise to experiment with Transformer models for the first time. The goal is to classify a written sentence as either positive or negative, using a BERT-based sequence classification model.

Although reducing the meaning of a sentence to only two categories can be simplistic, this project represents a useful first approach to Natural Language Processing (NLP), sentiment analysis, and Transformer-based models.

## Project objective

The objective of this project is to understand how a BERT model can be used for basic text classification.

The script performs the following steps:

1. Installs the required libraries.
2. Imports `torch` and Hugging Face `transformers`.
3. Loads the BERT tokenizer.
4. Loads a BERT sequence classification model.
5. Encodes an input sentence.
6. Runs the sentence through the model.
7. Prints whether the sentence is classified as positive or negative.

## Technologies used

- Python
- PyTorch
- Hugging Face Transformers
- BERT
- Google Colab / Jupyter Notebook

## Model used

The project uses:

```python
bert-base-uncased
```

through the following Hugging Face classes:

```python
BertTokenizer
BertForSequenceClassification
```

## How to run

### Option 1: Run the notebook

Open the notebook:

```text
classificazione_frasi_con_BERT_transformers.ipynb
```

and execute the cells in order.

This is the recommended option, especially if you are using Google Colab.

### Option 2: Run the Python script

Install the required libraries:

```bash
pip install transformers torch
```

Then run:

```bash
python classificazione_frasi_con_bert_transformers.py
```

## Project structure

```text
classificazione_frasi_con_BERT_transformers/
│
├── README.md
├── classificazione_frasi_con_BERT_transformers.ipynb
└── classificazione_frasi_con_bert_transformers.py
```

## Example workflow

The script takes a sentence as input, tokenizes it using the BERT tokenizer, converts it into input IDs, and sends it to the BERT model for classification.

The output is printed as:

```text
Positive review
```

or:

```text
Negative review
```

## Notes

This project is mainly educational. It is intended as a first experiment with Transformer models and sentence classification.

For a more accurate sentiment analysis project, the model should be fine-tuned on a labeled sentiment dataset, or replaced with a BERT model already fine-tuned for sentiment classification.

## Possible improvements

Future improvements could include:

1. Fine-tuning BERT on a real sentiment analysis dataset.
2. Adding a larger set of example sentences.
3. Creating a simple user interface for entering custom text.
4. Comparing BERT with other Transformer models.
5. Evaluating the model with accuracy, precision, recall, and F1-score.

## Author

Project developed as a personal exercise to learn the basics of BERT, Transformers, and sentence classification.
