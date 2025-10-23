🦾 YOLO11 Custom Training for Object Detection
This project demonstrates custom object detection using YOLO11.
The dataset is hosted on Roboflow, and training is performed in Google Colab.

📌 Features
Custom YOLO11 object detection training
Roboflow dataset integration
Training & evaluation in Google Colab
Reproducible pipeline with clear steps
📂 Dataset
Source: PPE Detection Dataset on Roboflow Universe

Classes (3):

🪖 Protective Helmet
🦺 Safety Vest
👢 Protective Boots
Format: YOLOv11-ready annotations

Splits: 70% Training | 20% Validation | 10% Testing

📥 Download in Colab
from roboflow import Roboflow

rf = Roboflow(api_key="YOUR_API_KEY")  # Replace with your Roboflow API key
project = rf.workspace("monitoring-rkejy").project("monitoring")
version = project.version(1)
dataset = version.download("yolov11")
⚠️ Replace "YOUR_API_KEY" with your Roboflow key.

🚀 How to Run
# Clone repository
git clone https://github.com/SudarshanG-coder/YOLO11-Custom-Training.git
cd YOLO11-Custom-Training

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook YOLO11_Custom_training_for_Object_Detection.ipynb
Results
Example evaluation metrics (replace with your actual results):

mAP@50: 0.87
mAP@50-95: 0.74
Precision: 0.82
Recall: 0.79
 



🌟 Key Highlights
End-to-end object detection workflow
High accuracy on PPE detection task
Easy dataset integration via Roboflow
Fully reproducible with Colab & Jupyter Notebook
 Future Improvements
Experiment with YOLO11 variations (Nano, Small, Medium, Large)
Hyperparameter tuning for better accuracy
Real-time detection deployment with OpenCV
Model export for Edge Devices (Jetson, Raspberry Pi, Mobile)
