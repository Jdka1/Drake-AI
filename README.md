# Drake-AI

<img src="{https://tinyurl.com/2p9ft7xf}" />


This repository contains a Jupyter notebook (`Song_Generation.ipynb`) for generating song lyrics using the dolly-v2-3b LLM. The notebook uses the Hugging Face `transformers` library for fine-tuning the model. 

Everything is 100% free to replicate using google colab compute and [this](https://docs.google.com/spreadsheets/d/e/2PACX-1vTjn49YWFG5pzoXyw7f4IU2TXw0vu0pCjHWc3k9qbd9MSADgr4SoGTljMKPblRWYo9xsAjOXD7ytUff/pub?output=csv) dataset created. 💯

**[Full Song](https://youtu.be/LeKcMHyd0m0)**

## Prerequisites

Before running the notebook, ensure that you have the required dependencies installed. You can install them using the following commands:

```bash
!pip install -q -U bitsandbytes
!pip install -q -U git+https://github.com/huggingface/transformers.git
!pip install -q -U git+https://github.com/huggingface/peft.git
!pip install -q -U git+https://github.com/huggingface/accelerate.git
!pip install -q datasets
```

Please note that there might be dependency conflicts, and you may need to resolve them based on the error messages.

## Data Preparation

The notebook downloads a dataset of Drake's lyrics from Kaggle using the Kaggle API. Make sure to provide your Kaggle API key and follow the instructions to secure it.

## Data Processing and Prompt Generation

The notebook processes the downloaded lyrics data, removes empty entries, and generates prompts for each song using OpenAI's GPT-3.5-turbo model.

## Loading Training Data

The notebook then loads the training data from a Google Sheets CSV that I have publicly postest for fine-tuning the model.

## Model Training

The model is fine-tuned on the prepared dataset using the `DrakeTrainer` class, a custom trainer based on the `transformers` library.

## Song Generation

The notebook demonstrates song generation using prompts. It provides examples of generating lyrics based on a given prompt and showcases the generated results.

## License

This project is licensed under the MIT License.

Feel free to explore, experiment, and create your own songs using this notebook!
