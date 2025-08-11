# Harmful-Brain-Activity-Classification-using-VGG16
Deep learning-based classification of harmful brain activity from EEG-derived spectrogram images using a custom VGG16 architecture
This project aims to assist in early diagnosis of neurological disorders like epilepsy.

**Features**

Custom VGG16 architecture adapted for spectrogram image classification.

Input preprocessing: resizing and normalization for VGG16.

Multi-class classification for harmful brain activity patterns.

Trained with optimized hyperparameters using Keras/TensorFlow.

Visualization of training curves and evaluation metrics.

**Dataset**

Source: HMS Harmful Brain Activity Classification dataset (Kaggle).

Format: EEG recordings converted into spectrogram images by the dataset provider.

Classes: 6 brain activity categories (harmful and non-harmful).

Resolution: Resized to 150×150 RGB format for VGG16.

**Methodology**

Data Loading & Preprocessing

Loaded spectrogram images from .parquet files.

Normalized pixel values and resized to 150×150.

Converted grayscale spectrograms to RGB.

**Model Architecture**

Modified VGG16 with custom input size (150×150×3).

Fully connected layers tuned for 6-class classification.

**Training**

Optimizer: RMSprop.

Loss: Categorical Crossentropy.

Early stopping and accuracy monitoring.

**Results**

Training Accuracy: 80%

Confusion matrix & classification report available in /results folder.

Model demonstrates strong performance on harmful brain activity detection but could benefit from further tuning and data augmentation.

**Future Work**

Experiment with ResNet, EfficientNet, and ensemble models.

Integrate real-time EEG stream classification.

Expand dataset for better generalization.

**Contact**

If you have questions, suggestions, or would like to discuss this project, feel free to email me at keerthisrinivas0507@gmail.com.
