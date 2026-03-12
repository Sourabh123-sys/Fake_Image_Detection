Fake Image Detection AI

Overview

Fake Image Detection AI is a multi-model deep learning system that detects whether an image is real or fake.
The system automatically analyzes the image type (face, building, or nature) and selects the best AI model to perform detection.

The project combines multiple deep learning models with an ensemble approach to improve detection accuracy.

Features

Multi-model AI detection system

Automatic image type detection

Face detection using MTCNN

Ensemble prediction from multiple models

Grad-CAM visualization for model explainability

Flask backend API

Web-based user interface for uploading images

Models Used
1. Face Detection Model

Architecture: FaceNet

Dataset: VGGFace2 pretrained weights

Used for detecting fake or manipulated face images

2. Building Detection Model
   
Architecture: EfficientNet-B4

Used for detecting fake building images

4. Nature Detection Model

Architecture: EfficientNet-B3

Used for detecting fake nature or landscape images

System Architecture
The system works in the following steps:

User uploads an image from the web interface.

The backend detects the type of image.

The appropriate model is selected automatically.

The model predicts whether the image is real or fake.

Grad-CAM generates visual explanations showing important regions.

Installation

1. Clone the repository
git clone https://github.com/Sourabh123-sys/Fake_Image_Detection.git
cd Fake_Image_Detection

3. Create virtual environment
python -m venv venv

Activate environment:

Windows
venv\Scripts\activate

Linux / Mac

source venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

Running the Application

Start the Flask server:

python app.py

Server will start at:

http://localhost:5001

Open the URL in your browser and upload an image.

Example Workflow

Upload an image through the web interface.

The system automatically detects the image type.

The AI model predicts if the image is real or fake.

Grad-CAM highlights important image regions.

Technologies Used

Python

PyTorch

OpenCV

Flask

NumPy

Pillow

FaceNet

EfficientNet

Future Improvements

Add transformer-based vision models

Improve ensemble accuracy

Deploy system as cloud API

Add video deepfake detection

<img width="1913" height="868" alt="image" src="https://github.com/user-attachments/assets/752eb759-7e88-4311-9077-d572802beb33" />



