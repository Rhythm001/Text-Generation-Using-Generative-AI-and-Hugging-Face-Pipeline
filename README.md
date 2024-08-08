# Text-Generation-Using-Generative-AI-and-Hugging-Face-Pipeline
A simple text generation AI using Mistral-7B-instruct, using GPU on Google Colab.

## Overview
This code demonstrates how to interact with HuggingFace models using the LangChain library within a Google Colab environment. It covers the process of securely managing API tokens, invoking language models, and utilizing GPU acceleration for text generation tasks.

### Key Components:
Environment Secret Keys Management:

API tokens are retrieved from Google Colab's secret storage and set as environment variables to securely access HuggingFace models.


### Accessing HuggingFace Models:

The HuggingFaceEndpoint class is used to connect to specific models on HuggingFace, such as "mistralai/Mistral-7B-Instruct-v0.2" and "mistralai/Mistral-7B-Instruct-v0.3".
Model parameters like max_length and temperature are set to control the output generation.


### Model Invocation:

The models are invoked with specific prompts to generate responses, demonstrating the model's ability to answer questions and perform step-by-step reasoning.
Examples include querying the capital of Himachal Pradesh and identifying the Prime Minister of Bangladesh.

### Prompt Templates and LLM Chains:

The code uses the PromptTemplate and LLMChain classes to create structured prompts and chain together different language model invocations for more complex tasks.

### Using HuggingFace Pipelines:

An alternative approach using HuggingFacePipeline allows for direct interaction with models such as GPT-2, with options to utilize hardware accelerators like GPUs for faster processing.
The pipeline is configured for text generation, and an example invocation demonstrates its usage.
GPU Acceleration:

Instructions are provided for enabling GPU usage in Colab, and the code demonstrates how to configure the HuggingFacePipeline for GPU-accelerated text generation tasks.
