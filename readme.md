# Retriever-Augmented Generation (RAG) on PubMed Database

This repository contains a Python notebook and a utility file (`utils.py`) that demonstrate the implementation of a Retriever-Augmented Generation (RAG) system applied to the PubMed database from Hugging Face.

## Files

- `RAG_on_PubMed.ipynb`: A Jupyter notebook that showcases the implementation of our RAG model on the PubMed dataset.
- `utils.py`: A utility file used by the notebook for various functions. This file is the same as the one provided by the Deeplearning.ai course "Building and Evaluating Advanced RAG".

## Implementation Overview

Our implementation focuses on developing RAG systems to effectively update doctors' knowledge. Our RAG model embeds chunks of our data collection into vectors using GPT-3.5, stores them in a vector database, and retrieves the most relevant chunks based on a query prompt. These chunks are then provided as context for answering the query.

We employed a labeled dataset of 1,000 queries from PubMed to evaluate the performance of our model. The evaluation metrics included groundedness, context relevance, and answer relevance, which were computed using TruEra.

## References

This implementation is based on concepts from the Deeplearning.ai course "Building and Evaluating Advanced RAG" by Jerry Liu and Anupam Datta. For more information, visit [the course page](https://www.deeplearning.ai/short-courses/building-evaluating-advanced-rag).

The PubMed dataset is available on Hugging Face: [PubMed Dataset](https://huggingface.co/datasets/pubmed)

## Usage

To use this repository, clone it to your local machine and open the `RAG_on_PubMed.ipynb` notebook in a Jupyter environment. Ensure you have all the necessary dependencies installed, as listed in requirements.txt.

Additional to those requirements, you also have to execute: 

`pip install llama-index-embeddings-huggingface`