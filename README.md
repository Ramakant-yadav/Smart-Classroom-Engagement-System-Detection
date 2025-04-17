# Smart Classroom: Student Engagement Detection using CNN

This project aims to detect student engagement levels from facial images using deep learning (CNNs) and computer vision. It classifies students into the following categories:

- Engaged
  - Engaged
  - Confused
  - Frustrated
- Not Engaged
  - Looking Away
  - Bored
  - Drowsy

## Dataset

Dataset used: Student Engagement Dataset  
Structure:
dataset/ ├── Engaged/ │   ├── confused/ │   ├── engaged/ │   └── frustrated/ └── Not engaged/ ├── Looking Away/ ├── bored/ └── drowsy/

After preprocessing, the dataset was flattened and split into:
- train/
- test/

## Model Architecture

A custom Convolutional Neural Network (CNN) was built using TensorFlow and Keras with the following components:

- Convolutional + MaxPooling layers
- Dropout for regularization
- Dense layers for classification
- softmax activation with sparse_categorical_crossentropy loss

## Results

- Training Accuracy: ~90%
- Test Accuracy: ~72%
- Test Loss: ~0.47

## Sample Predictions

Random test images are passed through the model, and predictions are visualized with:

- Predicted label (class)
- Ground truth label
- (Optional) Dlib-based face detection rectangles

## Features

- Custom CNN model using Keras
- Image preprocessing using OpenCV
- Face detection using Haar Cascades and Dlib CNN model
- Sample prediction visualizations
- Code modularized for easy deployment

## How to Run

1. Clone the repo and open in Google Colab
2. Upload the dataset zip
3. Run the notebook cells step-by-step:
   - Unzipping & preprocessing
   - Model training
   - Evaluation & visualization
4. (Optional) Upload custom images for prediction

## Next Steps

- Convert to TFLite for mobile deployment
- Build a Streamlit web interface
- Integrate real-time webcam prediction

## Author

Ramakant Yadav
[GitHub](https://github.com/Ramakant-yadav/) | [LinkedIn](https://www.linkedin.com/in/ramakant-yadav/)

---

*Presented as part of a Smart Classroom AI initiative. For research, academic, and experimental use only.*
