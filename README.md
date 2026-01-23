# 📘 COGNITIVE‑VIDEO‑RECOGNITION‑AD‑BUDDY

## 📌 Project Overview  
A computer vision system for **detecting and recognizing objects in video footage**, designed to assist with cognitive video analysis tasks like summarizing key moments and classifying activities or objects of interest. Built on **YOLOv8**, this project automates video understanding for research and real-world applications.

---

## 🧠 Features

- 🟦 **Object Detection in Videos** using YOLOv8  
- ▶️ **Video Processing & Inference** — batch processing of videos to extract detections  
- 🛠 **Modular Design** — separate modules for detection, tracking, and analysis  
- 📊 **Results Export** — bounding boxes and labels for further analysis or visualization  

---

## 📁 Repository Structure

COGNITIVE‑VIDEO‑RECOGNITION‑AD‑BUDDY/

┣ 📂src/ # Source code modules

┣ 📂models/ # Saved YOLOv8 models / configs

┣ 📂notebooks/ # Jupyter notebooks for demos

┣ 📄README.md # This file


> ⚠️ Note: Video datasets and results are **not included** due to size limits. See “External Results & Demos” below.

---

## ⚙️ Setup & Installation

1. Clone the repository:
```
git clone https://github.com/junaid-4001/COGNITIVE-VIDEO-RECOGNITION-AD-BUDDY.git
cd COGNITIVE-VIDEO-RECOGNITION-AD-BUDDY
```

2. Create a virtual environment (recommended):
```
python3 -m venv venv
source venv/bin/activate   # macOS / Linux
```

3. Install required Python packages:
'''
pip install ultralytics opencv-python numpy pandas matplotlib jupyter

## 🏃‍♂️ Running YOLOv8 Inference
# Detect objects in a video:
```
python src/detect.py --weights models/best.pt --source videos/input.mp4 --save-txt --save-conf
```

--weights → path to your YOLOv8 model

--source → input video or folder

--save-txt → saves detected labels

--save-conf → saves confidence scores

# Optional: Run on images
```
python src/detect.py --weights models/best.pt --source images/ --save-txt
```

## 📊 Jupyter Notebook Demos

-> notebooks/For pics.ipynb — test object detection on images

-> notebooks/For videos.ipynb — process videos using YOLOv8

-> notebooks/KeyWord_Extraction.ipynb — analyze labels for keyword extraction

## 📎 External Results & Demos

Video outputs cannot be stored in GitHub due to size limits. 
Sample results are hosted externally at:

## 📚 Technologies Used

Python 3

YOLOv8

OpenCV

NumPy, Pandas, Matplotlib
Jupyter Notebooks

