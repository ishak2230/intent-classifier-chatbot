# Intent Classifier Chatbot

A simple intent-based chatbot built with Python, NLTK, and TensorFlow. It uses a neural network to classify user input based on predefined categories (intents) and responds accordingly.

## Project Overview

This project demonstrates how natural language processing (NLP) and machine learning can work together to build a basic conversational agent. The chatbot:
- Processes user input using tokenization and stemming
- Converts input into a bag-of-words representation
- Uses a neural network to classify input into one of the known intents
- Responds with a predefined message for that intent

## How It Works

1. **Data Source**: The `intents.json` file contains different user intents with:
   - Tags (e.g., greeting, goodbye)
   - Example input patterns
   - Corresponding responses

2. **Preprocessing**:
   - Tokenization and stemming using `nltk`
   - Bag-of-words vector creation for training

3. **Model Training**:
   - A feedforward neural network using `tflearn` (built on TensorFlow)
   - Trained to classify input sentences into correct intent tags

4. **Prediction & Response**:
   - During chat, the model predicts the intent of the user message
   - If confidence > 70%, a random response for that tag is shown
   - Otherwise, a fallback message is used

## Installation

### Clone the repository
```bash
git clone https://github.com/yourusername/intent-classifier-chatbot.git
cd intent-classifier-chatbot
