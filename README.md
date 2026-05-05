TWEET EMOTION RECOGNITION WITH TENSORFLOW

This project focuses on classifying emotions in tweets using Recurrent Neural Networks (RNN) and TensorFlow. As a Biomedical Engineering student, I developed this project to understand the logic of sequence processing and deep learning models, which are also crucial for biomedical signal analysis (like EEG/ECG).

PROJECT OVERVIEW

The goal is to build and train a model that can categorize tweets into six different emotions: sadness, joy, love, anger, fear, and surprise.

TECH STACK

Language: Python

Library: TensorFlow / Keras

Data Processing: NumPy, Pandas, Tokenizer

Visualization: Matplotlib (Confusion Matrix, Accuracy/Loss Curves)

KEY LEARNING STEPS 

Data Pre-processing: Converting text to numeric tokens using Tokenizer and handling sequence lengths with pad_sequences.

Model Architecture: Building a Bidirectional LSTM (Long Short-Term Memory) network to capture the context of words in both directions.

Evaluation: Using a Confusion Matrix to analyze which emotions the model tends to confuse (e.g., joy vs. love).

CHALLENGES AND DEBUGGING (My Engineering Journey)

During this project, I encountered several technical challenges that I had to solve manually:

Legacy Code Updates: Fixed the AttributeError: 'Sequential' object has no attribute 'predict_classes' error by implementing the modern np.argmax(model.predict(x), axis=-1) method.

Data Type Handling: Resolved TypeError: data type 'uint8' not understood by ensuring proper NumPy data type declarations.

Label Mapping: Managed custom label dictionary mapping when the datasets library pre-encoded the labels.

RESULTS

The model achieved an accuracy of approximately 87% on the test set.

CONNECTING TO BIOMEDICAL ENGINEERING 

I aim to apply the sequence processing and RNN logic learned in this project to analyze biomedical time-series data (such as physiological signal classification) in future academic and professional projects.
