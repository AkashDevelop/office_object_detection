# 📹 CCTV-Based Attendance & Working-Hours Detection System  

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg?logo=python)](https://www.python.org/)  [![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-green)](https://github.com/ultralytics/ultralytics)  [![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-red)](https://opencv.org/)  [![Tesseract OCR](https://img.shields.io/badge/Tesseract-OCR-lightblue)](https://github.com/tesseract-ocr/tesseract)  [![FastAPI](https://img.shields.io/badge/FastAPI-Backend-teal)](https://fastapi.tiangolo.com/)  [![GPU](https://img.shields.io/badge/Compute-NVIDIA%20GPU-black)]()  

---

## 🎯 Objective  
This project automates **employee attendance tracking** and **working-hours calculation** from **live CCTV streams**.  
It uses **YOLOv8m** for person detection, **Tesseract OCR** for timestamp extraction, and a **GPU-powered pipeline** for real-time performance.  

---

## ✨ Features  
- 🔍 **Real-time Person Detection** from CCTV RTSP streams using YOLOv8m.  
- ⏱️ **Timestamp Extraction** with Tesseract OCR (achieved ~90% accuracy).  
- 🖥️ **GPU-Optimized Batch Inference** for faster frame processing.  
- 📊 Automatic **in-time, out-time, and total working-hours calculation**.  
- ⚡ End-to-end scalable pipeline (sampling + inference + integration).  

---

## 🛠️ Tech Stack  
- **Programming Language:** Python  
- **Frameworks & Libraries:** YOLOv8, OpenCV, Tesseract OCR, FastAPI  
- **Deployment:** GPU server (batch inference for optimized latency)  

---


---

## 🚀 Installation  

```bash
# Clone the repo
git clone https://github.com/AkashDevelop/office_object_detection.git
cd office_object_detection

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

## Usage 

# Run pipeline on RTSP stream
python src/pipeline.py --rtsp_url "rtsp://your_camera_url" --weights models/yolov8m.pt

