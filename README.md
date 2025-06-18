# 🚧 Road Safety Monitoring – AI-Based Pothole Detection and Size Estimation

This project aims to enhance road safety by detecting potholes using AI and estimating their size and severity. It combines object detection and depth estimation techniques to support automated maintenance decision-making.

## 📌 Problem Statement

Potholes are a major cause of road accidents and vehicle damage. Manual monitoring is inefficient and slow. Our system provides an automated solution using deep learning and computer vision to:

- Detect potholes in road images
- Estimate the **length**, **breadth**, and **depth**
- Classify severity levels
- Suggest approximate repair costs

---

## 🧠 Core Technologies

| Task | Technology Used |
|------|-----------------|
| Pothole Detection | YOLOv11 |
| Depth Estimation | MiDaS |
| Image Preprocessing | OpenCV |
| Frontend Interface | Streamlit |
| Data Handling | Pandas, NumPy |
| Deployment | Localhost / Web App (optional) |

---

## 📷 Features

- 🔍 **Pothole Detection** with bounding boxes using YOLOv11
- 📏 **Size Estimation** (Length, Breadth, Area, Perimeter)
- 📐 **Depth Map Generation** using MiDaS
- 📊 **Volume and Repair Cost Estimation**
- 🎯 **Severity Classification** (Low, Medium, High)
- 🧾 **CSV Report Generation**
- 🌐 **User Interface** for uploading and viewing results

---

## 🧪 Sample Workflow

1. **Upload Image** via Streamlit interface
2. **Detect potholes** using trained YOLOv11 model
3. **Generate depth map** using MiDaS
4. **Estimate dimensions** and calculate:
   - Volume
   - Average depth
   - Severity
   - Repair cost
5. **Save results** as annotated image + CSV row

---

## 📁 Project Structure

📂 pothole_project/
├── 📁 model/
│ └── best.pt (YOLOv11 weights)
├── 📁 utils/
│ ├── depth_estimation.py
│ ├── dimension_calculator.py
│ └── severity_classifier.py
├── 📁 output/
│ └── annotated_images, csv, etc.
├── app.py (Streamlit frontend)
├── detect.py (Main processing pipeline)
├── requirements.txt
└── README.md

yaml
Copy
Edit

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip
- Git

### Installation

```bash
git clone https://github.com/yourusername/pothole-detection.git
cd pothole-detection
pip install -r requirements.txt
Run the App
bash
Copy
Edit
streamlit run app.py
👨‍💻 Contributors
Syed Saleem
Thejas Babu R

Guide: Mr.Nitin Chaudhari
