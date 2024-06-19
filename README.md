
# Threatening Call Detection

This project is focused on detecting threatening calls by converting speech to text and using a fine-tuned DistilBERT model to classify the transcribed text as either a threat or non-threat.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
  - [Fine-tuning DistilBERT](#fine-tuning-distilbert)
  - [Threat Identification from Calls](#threat-identification-from-calls)
- [Configuration](#configuration)


## Introduction

This project leverages a fine-tuned DistilBERT model to classify transcribed speech from calls as either a threat or non-threat. The system captures audio input, converts it to text, and then uses the model to identify potential threats. Alerts are sent if a threat is detected.

## Features

- **Audio to Text Conversion**: Converts spoken language from calls to text using speech recognition.
- **Threat Detection**: Classifies the transcribed text as a threat or non-threat using a fine-tuned DistilBERT model.
- **Alerts**: Sends alerts if a threat is detected in the call.

## Usage

### Fine-tuning DistilBERT

1. Open `DistilBERT_finetuning.ipynb` in Google Colab or Jupyter Notebook.
2. Follow the instructions in the notebook to preprocess the data, fine-tune the DistilBERT model, and save the trained model.

### Threat Identification from Calls

1. Open `Threat_identifier.ipynb` in Google Colab or Jupyter Notebook.
2. Follow these steps in the notebook:
   - Capture audio input using a microphone.
   - Convert the audio input to text.
   - Use the fine-tuned DistilBERT model to classify the text.
   - Send an alert if a threat is detected.

## Configuration

- **Data Files**: Place your dataset files (`dataset.csv`, `Final_dataset.csv`, `data_threat.csv`) in the project directory.
- **Model and Tokenizer Paths**: Ensure the paths to the fine-tuned model and tokenizer in `Threat_identifier.ipynb` are correctly set to where the files are saved.
- **Alert Configuration**: Configure the phone numbers and message content in the `Threat_identifier.ipynb` for sending alerts.
