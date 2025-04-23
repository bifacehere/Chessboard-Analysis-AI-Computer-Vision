# 📄 README - Chessboard Analysis using AI & Computer Vision

## 🎯 Objective
The goal of this assignment is to create a computer vision solution that can accurately analyze a chessboard image—whether full or partial—and count the number of black and white squares. The program must be robust to variations in angle, lighting, and image quality.

## 🧠 Key Concepts Used
- Image Preprocessing (Grayscale, Gaussian Blur, Thresholding)
- Contour Detection
- Perspective Transformation
- Grid Segmentation
- Pixel Intensity Analysis

## 📚 Required Libraries
```bash
!pip install opencv-python-headless numpy matplotlib
```

Libraries used:
- `OpenCV`: for image reading, processing, and transformation
- `NumPy`: for numerical operations and array handling
- `Matplotlib`: for visualizing the image output in Colab

## 🚀 How to Use
1. Open this notebook in **Google Colab**.
2. Run the first code cell and **upload a chessboard image** (partial or full).
3. The script will display:
   - The original image
   - Thresholded grayscale image
   - Perspective corrected image (if applicable)
   - Final annotated image with black and white square count

## 📂 Folder Structure
```
📁 Chessboard-Analysis
├── 📓 Chessboard_Analysis.ipynb
├── 📷 test_images/
├── 📄 README.md
└── 🎥 demo_video_link.txt
```

## ✅ Features
- Detects full and partial chessboards
- Works with angled or slanted images
- Normalizes lighting using adaptive thresholding
- Performs perspective correction using contour detection
- Accurately counts black and white squares
- Visualizes the detected squares

## 📊 Output Example
- Annotated image showing 8x8 grid
- Printed results:
```
✅ Chessboard Square Count:
Black Squares: 32
White Squares: 32
```

## 📝 Evaluation Criteria Checklist
| Criteria            | Description                                           |
|---------------------|-------------------------------------------------------|
| Functionality        | Counts squares under various image distortions       |
| Robustness           | Handles slanted/angled/partial views and lighting    |
| Code Quality         | Modular, clean, well-documented                      |
| Creative Techniques  | Uses contour-based alignment + grid segmentation     |
| Result Presentation  | Annotated visuals and markdown explanations          |

## 📌 Summary for Non-Tech Reviewers
- The program loads a chessboard image and detects the board area.
- It corrects the angle or perspective if the board is slanted.
- It breaks the board into 64 segments (if possible).
- Each segment is analyzed to determine if it's black or white.
- The final image shows colored squares and counts of each type.

## 🎥 Demo Video
👉 **[Watch the demo video here](https://youtu.be/DYwbiH9H4wU?si=P2K6RBTusWxtgEk-)**

## 👨‍💻 Developer
**Sagar**  
BCA in AI & IoT  
Skilled in Python, AI, OpenCV, Scripting, and Problem Solving
