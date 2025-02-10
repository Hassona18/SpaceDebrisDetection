# Space Debris Detection using Detectron2

## 📌 Project Overview
This project utilizes **Detectron2**, a powerful object detection framework by Facebook AI, to detect and classify **space debris** in images. The model is trained using **Faster R-CNN**, a state-of-the-art object detection algorithm, and can be used to identify debris in space imagery.

## 📂 Dataset
The dataset for training and testing consists of images labeled with bounding boxes representing space debris. If you're using a publicly available dataset, ensure it's downloaded before training.

## 🛠️ Installation
To set up the project, follow these steps:

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/space-debris-detection.git
cd space-debris-detection
```

### 2️⃣ Install Dependencies
Ensure you have Python 3.8+ installed, then run:
```bash
pip install -r requirements.txt
```
Alternatively, install **Detectron2** separately using:
```bash
pip install 'git+https://github.com/facebookresearch/detectron2.git'
```

### 3️⃣ Download Dataset
Modify the dataset path in the script or download it from the source.

## 🚀 Training the Model
Run the following script to train the Faster R-CNN model:
```bash
python train.py
```
This will:
- Load the dataset
- Train the model using Faster R-CNN
- Save the trained weights

## 🏆 Making Predictions
After training, use the model to make predictions on new images:
```bash
python predict.py --image_path path/to/image.jpg
```
This script will:
- Load the trained model
- Detect space debris in the input image
- Display the results with bounding boxes

## 📷 Capturing Images with Google Colab
If using Google Colab, you can capture images from the webcam:
```python
from google.colab import files
uploaded = files.upload()
```
This will allow you to upload and test images in real-time.

## 📊 Visualizing Results
You can visualize detected objects with bounding boxes by running:
```bash
python visualize.py
```
This script will display images with detected debris and their confidence scores.

## 🔥 Future Improvements
- Train on a larger dataset for better accuracy
- Implement real-time video detection
- Optimize model inference for faster predictions

## 📝 License
This project is open-source under the MIT License. Feel free to contribute!

