# Drowsiness Detection Using YOLOv5 🚗💤

A real-time drowsiness detection system that evaluates whether a driver’s eyes are open or closed using webcam input. I used **YOLOv5**, **OpenCV**, **PyTorch**, and **Python** to deliver efficient and accurate detection.

## 📌 Project Goal

The primary objective of this project is to detect signs of driver drowsiness in real time by analyzing eye state using webcam video feed. If drowsiness is detected, the system can trigger alerts to help prevent accidents.

## ⚙️ Technologies Used

- **YOLOv5 (Ultralytics)** – Object detection for identifying facial features.
- **OpenCV** – For capturing and displaying real-time video frames.
- **PyTorch** – Deep learning framework used for training the model.
- **Python** – Primary programming language.
- **Jupyter Notebooks** – For development, training, and testing.
- **YAML** – To define model architecture and training parameters.

## 🔧 How It's Made

This project performs real-time object detection using a YOLOv5 model to detect human faces and classify eyes as open or closed.
1. **Video Input**: Frames are captured using OpenCV from the webcam.
2. **Detection**: Each frame is passed through the YOLOv5 model to locate and identify facial features.
3. **Rendering**: Detected faces and eye states are shown with bounding boxes.
4. **Loop**: The program runs in a loop until the user presses `'q'`.

## 📚 Project Workflow

### 1. Data Collection
Custom data for open/closed eyes was collected using a webcam and saved for training.

### 2. Data Annotation
The collected images were annotated using **LabelImg** to create bounding boxes for eye regions and assign appropriate labels.

### 3. Model Training
YOLOv5 was trained on the annotated dataset with fine-tuned hyperparameters such as image size, batch size, and epochs for optimal detection accuracy.

### 4. Real-Time Detection
Once trained, the model was deployed in a Python application using OpenCV to detect drowsiness in real time through webcam input.

## 🚀 Installation Instructions

!pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
### Clone YOLOv5 repo and install dependencies
!git clone https://github.com/ultralytics/yolov5
!cd yolov5
!pip install -r requirements.txt
