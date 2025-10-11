# Brain-Tumor-Detection-Using-Deep-Learning-MRI-Images-Detection-Using-Computer-Vision
🧠 Brain Tumour Detection Using Deep Learning
📘 Project Overview

This project is a Deep Learning–based Brain Tumour Detection System that classifies MRI scan images into multiple categories — determining whether a person has a brain tumour and identifying its stage.

The system provides a web-based interface built using HTML, CSS, and JavaScript, allowing users to upload MRI images easily. The backend is powered by Flask (Python), which handles image processing, model inference, and result visualization.

🚀 Features

🧩 Deep Learning Model: Detects the presence and type (or stage) of a brain tumour using a trained CNN model.

💻 Web Interface: Simple and responsive frontend for uploading and viewing MRI images.

⚙️ Flask Backend: Connects the deep learning model with the frontend for prediction.

📤 Image Upload & Preview: Users can select and preview MRI scans before submitting.

📊 Prediction Display: Results show whether the tumour is detected and its classification stage.

🗂️ Project Structure
Brain_Tumour_Detection/
│
├── static/
│   ├── css/
│   │   └── style.css           # Styling for the web app
│   ├── js/
│   │   └── script.js           # Frontend functionality for image upload & preview
│   └── images/                 # Sample MRI images (four types)
│
├── templates/
│   └── index.html              # Frontend HTML page
│
├── brain_tumour_detection_using_deep_learning.ipynb   # Jupyter Notebook for model training and testing
│
├── app.py                      # Flask backend script
│
├── model/
│   └── tumour_model.h5         # Trained deep learning model (saved)
│
└── README.md                   # Project documentation

🧠 Model Details

The Convolutional Neural Network (CNN) used in this project classifies MRI brain images into one of the following categories:

No Tumour

Glioma Tumour

Meningioma Tumour

Pituitary Tumour

The model was trained on a publicly available brain MRI dataset with image augmentation for better generalization.

🧩 Tech Stack
Component	Technology Used
Frontend	HTML, CSS, JavaScript
Backend	Flask (Python)
Model	TensorFlow / Keras
Environment	Jupyter Notebook
Language	Python
Deployment (optional)	Flask Server
⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/brain-tumour-detection.git
cd brain-tumour-detection

2️⃣ Install Dependencies

Make sure Python (≥3.8) and pip are installed, then run:

pip install -r requirements.txt


If you don’t have a requirements.txt, you can install manually:

pip install flask tensorflow keras numpy pandas opencv-python pillow

3️⃣ Run the Flask App
python app.py

4️⃣ Open in Browser

Visit:

http://127.0.0.1:5000/


Upload an MRI image to see the prediction result.

🧾 How It Works

The user uploads an MRI scan image through the web interface.

The Flask backend receives and preprocesses the image.

The CNN model predicts whether a tumour is present and identifies its type.

The result is displayed on the web interface.

🧪 Sample Images
Type	Description
Image 1	No Tumour
Image 2	Glioma Tumour
Image 3	Meningioma Tumour
Image 4	Pituitary Tumour

Each image is used to train and validate the model’s accuracy in classification.

📈 Future Improvements

Add explainable AI (Grad-CAM) for visualizing tumour detection regions.

Deploy the app using Docker or a cloud service (AWS, Heroku).

Add user authentication and patient record management.

👨‍💻 Author

Saurabh Sonare
Deep Learning Enthusiast | AI Developer
📧 saurabhsonare02@gmail.com
🔗 https://github.com/saurabh0426

🏷️ License

This project is licensed under the MIT License — feel free to use, modify, and distribute it for educational or research purposes.
