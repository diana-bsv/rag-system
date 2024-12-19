# Retrieval-Augmented Generation (RAG) System  

This project implements a Retrieval-Augmented Generation (RAG) system, which combines retrieval-based and generative approaches to enhance the quality and relevance of generated content.

## Overview

The RAG system is designed to retrieve relevant information from a database source and incorporate it into a generative model’s responses. This approach improves the relevance and accuracy of generated outputs, especially for complex or knowledge-intensive tasks.  

To identify the most relevant context from a database used K-Nearest Neighbors (KNN) method.  

Pretrained models used:
- [facebook/dpr-ctx_encoder-multiset-base](https://huggingface.co/facebook/dpr-ctx_encoder-multiset-base) for context encoding
- [facebook/dpr-question_encoder-multiset-base](https://huggingface.co/facebook/dpr-question_encoder-multiset-base) for question encoding
- [google/flan-t5-base](https://huggingface.co/google/flan-t5-base) for generating response based on the retrieved context

## Why RAG?

Traditional generative models rely solely on pre-trained knowledge, which can become outdated or insufficient. By incorporating real-time retrieval, the RAG system ensures:

- Improved Relevance. Dynamically retrieves up-to-date information.
- Accuracy. Enhances the precision of responses by grounding them in retrieved evidence.
- Scalability. Easily adaptable to various domains with different databases or knowledge sources.
