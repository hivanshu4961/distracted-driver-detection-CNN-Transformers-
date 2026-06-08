Distracted Driver Detection using CNNs and Transformers
Overview

This project classifies driver behavior from images to detect distracted driving activities. Multiple deep learning architectures were implemented and compared, including CNNs, transfer learning with MobileNet, and Vision Transformers. The final solution was deployed on Hugging Face Spaces for real-time inference through a simple web interface.

Dataset

The project uses the State Farm Distracted Driver Detection dataset from Kaggle, containing 10 driver activity classes. The training data was split into 80% training and 20% validation sets.

Models Evaluated
Baseline CNN
MobileNet (Transfer Learning)
Fine-Tuned MobileNet
Vision Transformer (ViT)
CNN + Transformer Hybrid
Results
Model	Validation Accuracy
Baseline CNN	>98%
Fine-Tuned MobileNet	~99%
Vision Transformer	~74%
CNN + Transformer Hybrid	~74%

Fine-Tuned MobileNet achieved the best performance, while Transformer-based models showed promising results after hyperparameter tuning but remained less effective than CNN-based approaches on this dataset.

Technologies Used
Python
TensorFlow / Keras
NumPy
OpenCV
Scikit-learn

Key Learnings
Transfer learning significantly improved model performance.
Fine-tuned MobileNet achieved the highest accuracy.
Learning rate tuning greatly improved Transformer performance.
Model performance is highly dependent on architecture choice and training configuration.

Future Work
Experiment with larger Vision Transformer architectures
Train on video sequences instead of individual images

Live Demo

The model has been deployed on Hugging Face Spaces, allowing to upload an image and receive real-time predictions of driver behavior.
link - https://huggingface.co/spaces/htyag/distracted-driver-detection
