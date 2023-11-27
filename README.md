# Song Generation with GPT-3.5-turbo

This repository contains a Jupyter notebook (`Song Generation.ipynb`) for generating song lyrics using OpenAI's GPT-3.5-turbo model. The notebook utilizes the Hugging Face `transformers` library for interacting with the model and the `accelerate` library for training acceleration.

## Prerequisites

Before running the notebook, ensure that you have the required dependencies installed. You can install them using the following commands:

```bash
!pip install -q -U bitsandbytes
!pip install -q -U git+https://github.com/huggingface/transformers.git
!pip install -q -U git+https://github.com/huggingface/peft.git
!pip install -q -U git+https://github.com/huggingface/accelerate.git
!pip install -q datasets openai
```

Please note that there might be dependency conflicts, and you may need to resolve them based on the error messages.

## Data Preparation

The notebook downloads a dataset of Drake's lyrics from Kaggle using the Kaggle API. Make sure to provide your Kaggle API key and follow the instructions to secure it.

## Data Processing and Prompt Generation

The notebook processes the downloaded lyrics data, removes empty entries, and generates prompts for each song using OpenAI's GPT-3.5-turbo model.

## Loading Training Data

The notebook loads additional training data from a Google Sheets CSV for fine-tuning the model.

## Model Setup

The notebook uses the `transformers` library to set up a GPT-3.5-turbo model for song generation. It also employs techniques such as gradient checkpointing and PEFT (Parameter Efficiency Training) for efficient training.

## Tokenization and Dataset Preparation

The notebook tokenizes the lyrics data, splits it into training and validation datasets, and prepares the data for training.

## Model Training

The GPT-3.5-turbo model is fine-tuned on the prepared dataset using the `DrakeTrainer` class, a custom trainer based on the `transformers` library.

## Song Generation

The notebook demonstrates song generation using prompts. It provides examples of generating lyrics based on a given prompt and showcases the generated results.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

Feel free to explore, experiment, and create your own songs using this notebook!
