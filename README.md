# Brain-Tumour-Prediction-Project
🧠 Brain Tumor Detection using CNN

This project focuses on detecting brain tumors from MRI scans using a Convolutional Neural Network (CNN).
The goal is to build a model that can automatically classify MRI images into two categories:

Tumor (Yes)

No Tumor (No)

By analyzing the patterns and textures within MRI images, the model helps in identifying whether a tumor is present or not. This kind of automation can assist medical professionals in the early detection of brain tumors.

📂 Project Overview

This repository contains all the files, data, and code used to train and test the CNN model for brain tumor prediction. The main Jupyter notebook includes every step — from importing the data and preprocessing it to building the CNN model, training it, and making predictions.

Folder Structure
Brain-Tumor-Detection/
│
├── Brain Tumor Prediction.ipynb   # Main notebook with code and model explanation
├── /dataset
│   ├── yes/                       # MRI images with tumor
│   └── no/                        # MRI images without tumor
├── /models                        # (Optional) Saved model files (.h5)
├── /results                       # (Optional) Contains evaluation results, plots, etc.
└── README.md                      # Project documentation (this file)

🧩 Dataset Details

The dataset consists of approximately 40 MRI brain scan images, categorized into two groups:

Yes → Images showing a brain tumor

No → Images showing no tumor

These MRI images are preprocessed before being fed into the model for training and testing.

Sample Images
Tumor	No Tumor

	
⚙️ Technologies Used

The project is entirely built using Python and several popular machine learning and image processing libraries:

🐍 Python

🧠 TensorFlow / Keras – for building and training the CNN model

📊 NumPy & Matplotlib – for data manipulation and visualization

🧩 OpenCV – for image reading and preprocessing

📈 Scikit-learn – for performance evaluation

🚀 How It Works

Data Preprocessing

Each MRI image is resized to a consistent shape (like 128×128 or 64×64).

Pixel values are normalized to make model training faster and more stable.

The dataset is divided into training and testing sets.

Model Architecture (CNN)

The model is built using multiple Convolutional Layers to extract features.

MaxPooling Layers are used to reduce spatial dimensions and prevent overfitting.

Fully connected Dense Layers help classify the extracted features.

The final output layer uses a Sigmoid activation function since this is a binary classification problem.

Training

The model is compiled using Binary Crossentropy loss and the Adam optimizer.

Training progress is tracked using accuracy as a performance metric.

Prediction

After training, the model can predict whether a newly provided MRI image shows a tumor or not.

📊 Results

Training Accuracy: ~95–98%

Testing Accuracy: ~90–95%

The model shows high accuracy and performs effectively in distinguishing between MRI scans with and without tumors.

🖼️ Example Predictions

When you pass an MRI image to the model, it outputs something like this:

Predicted: Tumor Detected ✅


or

Predicted: No Tumor Detected ❌


This simple and direct output makes it easy to interpret the model’s decision.

💡 Future Improvements

Here are a few ideas to make the project even better:

Increase the dataset size for improved model generalization.

Use Transfer Learning (e.g., with pre-trained models like VGG16, ResNet50).

Build a simple web application using Streamlit or Flask to upload and test MRI images in real time.

Add model explainability tools (like Grad-CAM) to visualize which parts of the MRI influenced the prediction.

🧑‍💻 Author

Saurabh
📧 saurabhsonare02@gmail.com
💼 Passionate about Artificial Intelligence, Machine Learning, and Computer Vision.

If you find this project helpful, feel free to ⭐ star the repository and contribute!

🪪 License

This project is open-source and available under the MIT License.
You are free to use, modify, and distribute it for educational or research purposes.
