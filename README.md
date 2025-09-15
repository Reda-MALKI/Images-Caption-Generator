Image Caption Generator
🔹 Overview

This project implements an image captioning system that automatically generates natural language descriptions for images. The approach combines deep learning for computer vision with sequence modeling for text generation.

The workflow is:

Feature Extraction – Pre-trained CNN (InceptionV3/VGG16) extracts visual features from input images.

Sequence Modeling – An LSTM-based language model learns to generate captions word by word, conditioned on the extracted features.

Training Strategy – The model is trained on paired (image, caption) datasets, with teacher forcing and sliding window sequences.

Caption Generation – At inference time, captions are generated iteratively using greedy decoding.

🔹 Key Features

Uses transfer learning with a pre-trained CNN for efficient image feature extraction.

Employs LSTM networks to capture temporal dependencies in text sequences.

Supports preprocessing pipelines: image resizing, tokenization, and sequence padding.

Provides functions for training, evaluation, and caption generation.

Demonstrates on real image datasets with qualitative results.

🔹 Tech Stack

Python 3

TensorFlow / Keras (deep learning models)

NumPy, Pandas (data preprocessing)

Matplotlib / PIL (image visualization & handling)

🔹 Limitations & Future Work

While LSTMs perform well, they face issues such as vanishing gradients and limited long-term context understanding.

➡️ Future Plan: Once the required hardware for Transformer-based architectures is available, this project will be extended with a Transformer + Attention mechanism to achieve more accurate and coherent captions.
