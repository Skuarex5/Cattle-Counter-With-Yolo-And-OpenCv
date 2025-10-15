# 🐄 Automatic Livestock Counting with YOLOv8 + Open CV  

---

## 📘 Description

This project implements a web-based system for **automatic detection, tracking, and counting of livestock** (cows, horses, and sheep) in videos using **YOLOv8**, **OpenCv** and **Flask** as the backend server.

---

## 🚀 Features

1. **Video upload:**  
   Users can upload one or more videos through a web interface (`index.html`).

2. **YOLOv8 processing:**  
   - Performs object detection and tracking frame by frame.  
   - If a GPU is available, it runs on **CUDA** with `half precision` for faster inference.  

3. **Smart counting:**  
   - Each detected animal receives a persistent tracking ID.  
   - Only stable detections (visible for at least 3 frames) are counted.  
   - Displays the maximum number of individuals per class detected during the video.  

4. **Live streaming:**  
   - The processed video is displayed in real time with bounding boxes and labels.  
   - Counts update dynamically through `/get_totales` requests.

---

## 🧠 Core Technologies

- **Python 3.11+**  
- **Flask** → lightweight web framework for routing and server logic.  
- **OpenCV (cv2)** → video processing and frame rendering.  
- **Ultralytics YOLOv8** → object detection and tracking engine.  
- **PyTorch** → deep learning framework with GPU (CUDA) support.  

---

## 📂 Project Structure

