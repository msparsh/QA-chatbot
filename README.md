# QA-chatbot

A Question-Answering chatbot implementation using BERT transformer model for extractive question answering from contextual text.

## Overview

This project demonstrates a simple yet powerful question-answering system built using the Hugging Face Transformers library. The chatbot can read a given context and extract precise answers to questions based on that context.

## Model

The project uses the **BERT-large** model fine-tuned on SQuAD dataset:
- **Model**: `bert-large-uncased-whole-word-masking-finetuned-squad`
- **Task**: Question Answering (Extractive)
- **Framework**: Hugging Face Transformers

## Dependencies

```python
transformers
```

Install the required library:
```bash
pip install transformers
```

## How It Works

The notebook demonstrates the following steps:

1. **Import the pipeline**: Load the question-answering pipeline from the transformers library
2. **Initialize the model**: Set up BERT-large model fine-tuned on SQuAD
3. **Provide context**: Supply a text passage containing relevant information
4. **Ask a question**: Query the model with a specific question about the context
5. **Get answer**: Receive the extracted answer with a confidence score

## Input/Output

### Input
- **question** (str): The question to be answered
- **context** (str): The text passage containing information relevant to the question

### Output
- **answer** (str): The extracted answer from the context
- **score** (float): Confidence score ranging from 0 to 1

## License

Apache-2.0 License
