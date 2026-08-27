# fresh-vs-rotten-dip-project-id-242006222e

# 🍎 Fresh vs Rotten Fruit Image Classification Using CNN

## Digital Image Processing Group Project
## Dataset url: https://huggingface.co/datasets/Project-AgML/fresh_rotten_fruit_classification
## GitURL: https://github.com/sehanMasstech/fresh-vs-rotten-dip-project-id-242006222e
## ColabURL: https://colab.research.google.com/drive/1nyds65iKm6Xw92TfbirIncrbaR7e_lp-?usp=sharing

---

## 👨‍🎓 Student Information

| Information | Details |
|---|---|
| **Student Name** | MD. Hasnahin Sehan |
| **Student ID** | 242006222e |
| **Section** | 1 |
| **Group** | Individual / Solo |
| **Course** | Digital Image Processing |
| **Project Type** | Binary Image Classification |

---

# 📌 1. Project Overview

This project implements a **binary image classification system** for identifying whether a fruit is **Fresh** or **Rotten** using a **Convolutional Neural Network (CNN)**.

The system takes a fruit image as input and predicts one of two classes:

```text
Fruit Image
     │
     ▼
 Image Preprocessing
     │
     ▼
 Data Augmentation
     │
     ▼
 Convolutional Neural Network
     │
     ▼
 Binary Classification
     │
     ├── Fresh
     │
     └── Rotten

The project demonstrates a complete digital image processing and deep learning workflow, including:

Dataset collection
Dataset exploration
Image visualization
Class distribution analysis
Train/validation/test splitting
Image resizing
RGB conversion
Pixel normalization
Data augmentation
CNN architecture design
Model training
Validation
Testing
Accuracy and loss analysis
Confusion matrix
Precision
Recall
F1-score
Sample predictions
Trained model saving

🎯 2. Project Objective

The main objective of this project is to develop a CNN-based computer vision system capable of distinguishing between fresh and rotten fruits.

The project is formulated as a binary image classification problem:

Class 0 → Fresh
Class 1 → Rotten

The trained model learns visual characteristics from fruit images and uses those learned features to classify previously unseen images.

💡 3. Why Fresh vs Rotten Fruit?

Freshness is an important factor in fruit quality.

Fresh and rotten fruits can often have visually different characteristics, including:

Color changes
Dark spots
Discoloration
Surface damage
Texture changes
Visible signs of spoilage

These characteristics make the problem suitable for computer vision and image classification.

The project was also selected because it satisfies the requirement for a binary image classification task while being different from the common Cats vs Dogs classification example.

🛠️ 4. Technologies Used

The following technologies and libraries were used to develop this project.

| Technology                | Purpose                              | Why It Was Used                                                                     |
| ------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------- |
| **Python**                | Main programming language            | Provides a large ecosystem for machine learning, image processing and data analysis |
| **Google Colab**          | Development and training environment | Provides an easy-to-use notebook environment with GPU acceleration                  |
| **TensorFlow**            | Deep learning framework              | Provides tools for building and training CNN models using GPU acceleration          |
| **Keras**                 | Neural-network API                   | Makes CNN architecture, training, evaluation and model saving easier                |
| **NumPy**                 | Numerical computation                | Used for image arrays, pixel normalization and numerical operations                 |
| **Pillow (PIL)**          | Image processing                     | Used for loading, converting and resizing images                                    |
| **Hugging Face Datasets** | Dataset loading                      | Provides direct access to the publicly available fruit dataset                      |
| **Scikit-learn**          | Machine learning utilities           | Used for data splitting and evaluation metrics                                      |
| **Matplotlib**            | Data visualization                   | Used for training graphs and sample prediction visualization                        |
| **Seaborn**               | Visualization                        | Used to create the confusion matrix heatmap                                         |
| **GitHub**                | Repository and submission            | Used to store and submit the complete project                                       |

🐍 5. Why Python?

Python was selected because it has a large ecosystem of libraries specifically designed for:

Artificial intelligence
Machine learning
Deep learning
Image processing
Numerical computation
Data visualization

Python also allows all the technologies used in this project to work together easily.

☁️ 6. Why Google Colab?

Google Colab was used as the main development and training environment.

CNN training involves many mathematical operations and can benefit significantly from GPU acceleration.

Google Colab provides:

Python environment
GPU acceleration
Jupyter-style notebooks
Easy package installation
Data visualization
Integration with Hugging Face

During development, TensorFlow successfully detected a GPU.

The project was trained using a GPU environment with a Tesla T4 GPU.

🧠 7. Why TensorFlow?

TensorFlow was selected as the primary deep learning framework because it provides the functionality required to:

Build CNN models
Train neural networks
Perform image preprocessing
Apply data augmentation
Use GPU acceleration
Evaluate models
Save trained models

TensorFlow also provides the Keras API, which makes developing neural networks easier.

Official documentation:

https://www.tensorflow.org/tutorials/images/classification

🔧 8. Why Keras?

Keras is used through TensorFlow to create and train the CNN.

It provides easy-to-use implementations of:

Conv2D
MaxPooling2D
BatchNormalization
Dense
Dropout
Flatten
Data augmentation layers

Keras also provides simple functions such as:

model.compile()
model.fit()
model.evaluate()
model.predict()
model.save()

This makes it suitable for implementing the complete machine-learning pipeline.

🔢 9. Why NumPy?

NumPy was used for numerical operations and manipulation of image data.

Images are represented as numerical arrays, so NumPy is useful for:

Converting images to arrays
Pixel normalization
Preparing input data
Numerical calculations

The project converts pixel values from:

0 – 255

to

0 – 1

🖼️ 10. Why Pillow?

Pillow (PIL) was used for image processing.

It was used to:

Load images
Convert images to RGB
Resize images
Convert image data into arrays

The final CNN input size is:

128 × 128 × 3
where:

128 = image height
128 = image width
3   = RGB channels

📊 11. Why Scikit-learn?

Scikit-learn was used for dataset splitting and model evaluation.

It provides implementations for:

Train/test splitting
Accuracy
Precision
Recall
F1-score
Confusion matrix
Classification report

These metrics provide more information about the model than accuracy alone.

📈 12. Why Matplotlib?

Matplotlib was used for visualizing the model's performance.

It was used to generate:

Training accuracy curves
Validation accuracy curves
Training loss curves
Validation loss curves
Sample prediction visualizations
🔥 13. Why Seaborn?

Seaborn was used to create a heatmap of the confusion matrix.

The heatmap makes it easier to understand how many images were correctly and incorrectly classified.

📦 14. Dataset
Fresh Rotten Fruit Classification Dataset

This project uses the publicly available:

Fresh Rotten Fruit Classification Dataset

Dataset Provider

Project-AgML

Dataset Platform

Hugging Face

Official Dataset

https://huggingface.co/datasets/Project-AgML/fresh_rotten_fruit_classification

📚 15. Dataset Statistics

The raw dataset used in this project contains:

Total Images: 3,200

The classes are evenly distributed:

Fresh  = 1,600
Rotten = 1,600

| Class     |    Images | Percentage |
| --------- | --------: | ---------: |
| Fresh     |     1,600 |        50% |
| Rotten    |     1,600 |        50% |
| **Total** | **3,200** |   **100%** |

The dataset contains images from multiple fruit types.

The dataset records include:

image
label
fruit_type

The classification labels used in this project are:

Label 0 → Fresh
Label 1 → Rotten
🎯 16. Why This Dataset Was Selected

This dataset was selected because:

1. It directly matches the project

The dataset already contains the required binary categories:

Fresh
Rotten
2. It contains enough images

The assignment recommends approximately 200 images per class or more.

This dataset provides:

1,600 Fresh images
1,600 Rotten images

Therefore, it significantly exceeds the recommended minimum.

3. It is balanced

Both classes contain exactly 1,600 images.

This creates a balanced binary classification problem.

4. It is publicly available

The dataset is publicly available through Hugging Face.

5. It contains multiple fruit types

The dataset covers multiple fruit types, making the task more meaningful than training on only one type of fruit.

🔄 17. Raw Dataset vs Augmented Dataset

The dataset provides both raw and augmented versions.

For this project, the raw dataset containing 3,200 images was used.

The reason for using the raw dataset is that data augmentation was implemented independently within the TensorFlow training pipeline.

This allows the project to demonstrate its own image preprocessing and augmentation techniques.

📜 18. Dataset Source and Citation
Hugging Face Dataset

Project-AgML — Fresh Rotten Fruit Classification

https://huggingface.co/datasets/Project-AgML/fresh_rotten_fruit_classification

Original Research

Sultana, N., Jahan, M., & Uddin, M. S. (2022).

An extensive dataset for successful recognition of fresh and rotten fruits.

Data in Brief, Volume 44, Article 108552.

DOI:

https://doi.org/10.1016/j.dib.2022.108552

Original Dataset

Sultana, N., Jahan, M., & Uddin, M. S. (2022).

Fresh and Rotten Fruits Dataset for Machine-Based Evaluation of Fruit Quality.

Mendeley Data, V1.

DOI:

https://doi.org/10.17632/bdd69gyhv8.1

Dataset License

The dataset is listed under the:

CC BY 4.0

license.

🔍 19. Dataset Exploration

Before training, the dataset was inspected to verify:

Total number of images
Number of classes
Class distribution
Fruit types
Image dimensions
Sample images
Label values

The dataset was confirmed to contain:

3,200 images

1,600 Fresh
1,600 Rotten

Sample images were also visualized to inspect the dataset.

| Dataset    |    Images | Percentage |
| ---------- | --------: | ---------: |
| Training   |     2,240 |        70% |
| Validation |       480 |        15% |
| Testing    |       480 |        15% |
| **Total**  | **3,200** |   **100%** |

The split was performed while maintaining the class distribution.

🏋️ 21. Training Dataset

The training set contains:

2,240 images

These images were used to train the CNN and update its learnable parameters.

🔎 22. Validation Dataset

The validation set contains:

480 images

Validation data was used during training to monitor how well the model generalizes to images that were not directly used to update the model weights.

🧪 23. Testing Dataset

The test set contains:

480 images

The test dataset was kept separate from model training and was used for final performance evaluation.

The test set contains:

240 Fresh
240 Rotten
🖼️ 24. Image Preprocessing

The original dataset contains high-resolution images.

For example, some images are approximately:

4160 × 3120 pixels

Using the original resolution would require significantly more memory and computational resources.

Therefore, images were resized to:

128 × 128 pixels
🌈 25. RGB Conversion

Images were converted into RGB format.

RGB consists of three color channels:

Red
Green
Blue

Therefore, each CNN input has the shape:

128 × 128 × 3
📐 26. Pixel Normalization

Images originally contain pixel values between:

0 – 255

The pixel values were normalized to:

0 – 1

using:

image = image / 255.0

Normalization helps provide input values in a smaller and consistent numerical range for neural-network training.

The preprocessing pipeline was verified with:

Image batch shape:
(32, 128, 128, 3)

Label batch shape:
(32,)

Pixel minimum:
0.0

Pixel maximum:
1.0
🔄 27. Data Augmentation

Data augmentation was applied to the training images.

The augmentation pipeline includes techniques such as:

Random horizontal flipping
Random rotation
Random zoom
Random contrast

These transformations create variations of training images while preserving the original classification.

💡 28. Why Data Augmentation?

A CNN can overfit when it repeatedly sees the same images.

Data augmentation increases the variety of images available during training.

For example:

Original Image
      │
      ├── Horizontal Flip
      ├── Rotation
      ├── Zoom
      └── Contrast Variation

This helps the model learn features that are less dependent on a specific image orientation or appearance.

Official TensorFlow documentation:

https://www.tensorflow.org/tutorials/images/data_augmentation

🧠 29. Why CNN?

A Convolutional Neural Network was selected because CNNs are designed specifically for image data.

CNNs can automatically learn spatial features from images.

Early layers can learn simple features such as:

Edges
Lines
Textures

Deeper layers can learn more complex visual patterns such as:

Fruit surface characteristics
Spots
Discoloration
Shapes
Texture patterns

Therefore, a CNN is well suited for distinguishing fresh and rotten fruits.

🏗️ 30. CNN Architecture

The project uses a custom CNN architecture.

Input Image
128 × 128 × 3
        │
        ▼
Data Augmentation
        │
        ▼
Conv2D
32 Filters
3 × 3
ReLU
        │
        ▼
Batch Normalization
        │
        ▼
Max Pooling
        │
        ▼
Conv2D
64 Filters
3 × 3
ReLU
        │
        ▼
Batch Normalization
        │
        ▼
Max Pooling
        │
        ▼
Conv2D
128 Filters
3 × 3
ReLU
        │
        ▼
Batch Normalization
        │
        ▼
Max Pooling
        │
        ▼
Conv2D
256 Filters
3 × 3
ReLU
        │
        ▼
Batch Normalization
        │
        ▼
Max Pooling
        │
        ▼
Flatten
        │
        ▼
Dense
256 Neurons
ReLU
        │
        ▼
Dropout
0.5
        │
        ▼
Dense
1 Neuron
Sigmoid
        │
        ▼
Fresh / Rotten
🔬 31. CNN Components
Conv2D

Convolutional layers extract visual features from images.

ReLU

ReLU introduces non-linearity into the network.

Batch Normalization

Batch normalization helps stabilize the training process.

Max Pooling

Max pooling reduces spatial dimensions while retaining important features.

Flatten

Flatten converts the extracted feature maps into a one-dimensional vector.

Dense Layer

The dense layer combines the learned features for classification.

Dropout

Dropout is used to reduce overfitting.

Sigmoid

The final sigmoid layer produces a probability for the binary classification.

📈 32. Increasing Feature Complexity

The CNN gradually increases its number of filters:

32 → 64 → 128 → 256

This allows the network to learn increasingly complex visual features as information moves deeper into the network.

🎲 33. Binary Classification Output

The final layer uses:

Dense(1, activation="sigmoid")

The sigmoid function produces a value between:

0 and 1

The classification is interpreted as:

Probability < 0.5
        ↓
      Fresh

Probability ≥ 0.5
        ↓
      Rotten
⚙️ 34. Model Compilation

The CNN was compiled using:

Optimizer:
Adam

Loss Function:
Binary Cross-Entropy

Metrics:
Accuracy
Precision
Recall
🚀 35. Why Adam Optimizer?

Adam was selected because it is a widely used optimizer for training neural networks.

It automatically adapts the learning rate during training and combines adaptive learning-rate methods with momentum-based optimization.

📉 36. Why Binary Cross-Entropy?

The project contains exactly two classes:

Fresh
Rotten

Therefore, binary cross-entropy is appropriate for measuring the difference between the actual class and the predicted probability.

📦 37. Batch Size

The model uses a batch size of:

32

The input batch was verified as:

Image batch shape:
(32, 128, 128, 3)

Label batch shape:
(32,)
⏹️ 38. Training Control

Training includes mechanisms for monitoring validation performance.

Early stopping can prevent unnecessary training when validation performance stops improving.

Learning-rate reduction can also be used to allow smaller updates when the model approaches a better solution.

📊 39. Training Performance

The training process records:

Training accuracy
Validation accuracy
Training loss
Validation loss

These values are visualized using graphs.

📈 40. Accuracy Curve

The accuracy graph shows how the training and validation accuracy changed during training.

📉 41. Loss Curve

The loss graph shows how the training and validation loss changed during training.

🧪 42. Final Test Results

After training, the model was evaluated using the separate test dataset.

The final results were:

| Metric        |     Result |
| ------------- | ---------: |
| **Test Loss** | **0.1135** |
| **Accuracy**  | **95.21%** |
| **Precision** | **96.57%** |
| **Recall**    | **93.75%** |
| **F1 Score**  | **95.14%** |

🎯 43. Accuracy

The CNN achieved:

95.21% Test Accuracy

on 480 unseen test images.

The model correctly classified:

457 / 480 images

and incorrectly classified:

23 / 480 images
📋 44. Classification Report
              precision    recall  f1-score   support

Fresh           0.9393    0.9667    0.9528       240
Rotten          0.9657    0.9375    0.9514       240

accuracy                            0.9521       480
macro avg       0.9525    0.9521    0.9521       480
weighted avg    0.9525    0.9521    0.9521       480
🔢 45. Confusion Matrix

The final confusion matrix is:

                 Predicted

                 Fresh    Rotten

Actual Fresh      232       8

Actual Rotten      15      225

The visualized confusion matrix is available below.

🔍 46. Confusion Matrix Interpretation
Actual Fresh
232 → Correctly classified as Fresh
8   → Incorrectly classified as Rotten
Actual Rotten
225 → Correctly classified as Rotten
15  → Incorrectly classified as Fresh

Therefore:

Correct Predictions:
232 + 225 = 457

Incorrect Predictions:
8 + 15 = 23
📐 47. Precision

Precision measures how reliable the positive predictions are.

The Rotten class achieved:

96.57% Precision

This means that when the model predicted Rotten, the prediction was correct at a high rate.

🔎 48. Recall

Recall measures how many actual examples of a class were correctly identified.

The Rotten class achieved:

93.75% Recall

The Fresh class achieved:

96.67% Recall
🏆 49. F1 Score

The final F1 score was:

95.14%

F1-score combines precision and recall into a single metric.

A high F1 score indicates that the model performs well across both classes.

🖼️ 50. Sample Predictions

Sample predictions generated by the trained CNN are shown below.

The visualization compares the predicted class with the actual class for multiple test images.

💾 51. Saved Model

The trained CNN model was saved as:

fresh_rotten_fruit_cnn.keras

The saved model can be loaded using:

import tensorflow as tf

model = tf.keras.models.load_model(
    "fresh_rotten_fruit_cnn.keras"
)
🧪 52. Example Prediction

A new fruit image can be processed using the following approach:

from PIL import Image
import numpy as np

image = Image.open("fruit.jpg").convert("RGB")

image = image.resize((128, 128))

image = np.array(
    image,
    dtype=np.float32
)

image = image / 255.0

image = np.expand_dims(
    image,
    axis=0
)

prediction = model.predict(image)

probability = prediction[0][0]

if probability >= 0.5:
    print("Prediction: Rotten")
else:
    print("Prediction: Fresh")
📁 53. Project Structure

The GitHub repository is organized as follows:

Fresh-Rotten-Fruit-CNN/
│
├── Fresh_Rotten_Fruit_CNN.ipynb
│
├── fresh_rotten_fruit_cnn.keras
│
├── README.md
│
├── requirements.txt
│
└── outputs/
    │
    ├── accuracy_curve.png
    ├── loss_curve.png
    ├── confusion_matrix.png
    └── sample_predictions.png
📦 54. Requirements

The main Python libraries required by the project are:

tensorflow
numpy
matplotlib
seaborn
scikit-learn
datasets
Pillow
▶️ 56. How to Run

The complete project implementation is provided in:

Fresh_Rotten_Fruit_CNN.ipynb

The notebook can be opened using:

Google Colab
Jupyter Notebook
JupyterLab

The notebook performs the complete workflow:

1. Import libraries
2. Load dataset
3. Explore dataset
4. Analyze class distribution
5. Visualize sample images
6. Split dataset
7. Preprocess images
8. Normalize images
9. Apply data augmentation
10. Build CNN
11. Compile model
12. Train model
13. Plot accuracy/loss
14. Evaluate test dataset
15. Generate predictions
16. Generate classification report
17. Generate confusion matrix
18. Generate sample predictions
19. Save trained model
⚠️ 57. Limitations

Although the model achieved 95.21% test accuracy, the system has some limitations.

Its performance may change when it receives images that are significantly different from the training dataset.

Possible factors include:

Different lighting conditions
Different cameras
Different backgrounds
Different fruit varieties
Different image quality
Unusual viewing angles
Blur
Different spoilage patterns

Therefore, this project is intended as an academic deep-learning and digital image processing project rather than a professional food-quality inspection system.

🚀 58. Future Improvements

Several improvements could be made in future versions.

Larger Dataset

A larger and more diverse dataset could improve generalization.

Transfer Learning

Pre-trained CNN architectures could be investigated, such as:

MobileNetV2
ResNet
EfficientNet
Higher Resolution

Higher-resolution inputs could preserve additional visual details.

Real-Time Classification

The trained model could be connected to a camera for real-time fruit classification.

Mobile Application

The model could be converted for mobile deployment.

Web Application

A web interface could allow users to upload fruit images and receive a Fresh/Rotten prediction.

📝 59. Conclusion

This project successfully implements a complete binary image classification system for distinguishing between fresh and rotten fruits.

A publicly available dataset from Project-AgML was used through Hugging Face.

The raw dataset contains:

3,200 total images

1,600 Fresh
1,600 Rotten

The dataset was divided into:

2,240 Training images
480 Validation images
480 Testing images

The images were processed using:

RGB conversion
128 × 128 resizing
Pixel normalization
Data augmentation

A custom Convolutional Neural Network was developed using TensorFlow and Keras.

The final model achieved:

Accuracy  = 95.21%
Precision = 96.57%
Recall    = 93.75%
F1 Score  = 95.14%

The model correctly classified:

457 out of 480

unseen test images.

The project demonstrates how digital image processing, computer vision and deep learning can be combined to automatically classify fruit images according to freshness.

📚 60. References
Dataset

Project-AgML.

Fresh Rotten Fruit Classification

https://huggingface.co/datasets/Project-AgML/fresh_rotten_fruit_classification

Original Research Paper

Sultana, N., Jahan, M., & Uddin, M. S. (2022).

An extensive dataset for successful recognition of fresh and rotten fruits.

Data in Brief, Volume 44, Article 108552.

https://doi.org/10.1016/j.dib.2022.108552

Original Dataset

Sultana, N., Jahan, M., & Uddin, M. S. (2022).

Fresh and Rotten Fruits Dataset for Machine-Based Evaluation of Fruit Quality.

Mendeley Data, V1.

https://doi.org/10.17632/bdd69gyhv8.1

TensorFlow Image Classification

TensorFlow.

Image Classification

https://www.tensorflow.org/tutorials/images/classification

TensorFlow Data Augmentation

TensorFlow.

Data Augmentation

https://www.tensorflow.org/tutorials/images/data_augmentation
