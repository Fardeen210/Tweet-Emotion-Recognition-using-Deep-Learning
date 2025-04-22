# Tweet-Emotion-Recognition-using-Deep-Learning

# 🚀 Project Overview
This repository hosts a deep learning pipeline for Tweet Emotion Recognition — classifying short social media posts into emotional categories such as joy, anger, fear, sadness, love, and surprise. The project leverages modern NLP tools and deep learning frameworks (TensorFlow & HuggingFace datasets) to create an efficient, scalable emotion classification system.

This project is based on a real-world dataset sourced from dair-ai / emotion and aims to demonstrate state-of-the-art performance on multi-class text classification.

# 💡 Project Highlights
Dataset: dair-ai/emotion — a clean, pre-labeled tweet dataset.

Model Architecture: Multi-layer feedforward neural network.

Sampling Strategy: Random sampling (20,000 samples) to ensure balanced representation and efficient computation.

Training Framework: TensorFlow / Keras.

Evaluation Metrics: Accuracy, Confusion Matrix, Validation Loss.

Achieved Accuracy: ~90% on the validation set.


# 📊 Dataset Description
Source: dair-ai / emotion
This dataset contains thousands of English tweets annotated with one of the following emotional labels:
Label Index	Emotion
0	sadness
1	joy
2	love
3	anger
4	fear
5	surprise

# Sample Data
Tweet	Emotion
"i love my new phone!"	joy
"i feel so lonely today."	sadness
"this is absolutely terrifying."	fear

# 🧠 Model Architecture
The core of this project is a Bidirectional LSTM (Long Short-Term Memory) neural network, built using TensorFlow. This architecture allows the model to capture both past (backward) and future (forward) context in a sequence, which is crucial for understanding the nuanced emotional tone in short social media texts.

# Architecture Overview:
Embedding Layer: Converts input tweets into dense vector representations.
Bidirectional LSTM Layer: Reads sequences in both forward and backward directions, capturing contextual relationships across the entire tweet.
Dense Layer(s): Fully connected layer(s) with ReLU activation to learn higher-order features.
Output Layer: Softmax activation for multi-class emotion classification

# ✅ Model Performance
Training Accuracy: ~92%
Validation Accuracy: ~90%
Confusion Matrix Analysis: Shows good balance across emotion classes with minor confusion between similar emotions (e.g., joy vs love).
Performance plots and the confusion matrix are available in the notebook for deeper insights.
