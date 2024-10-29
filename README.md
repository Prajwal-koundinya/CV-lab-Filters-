
---

# 🌌 Image Processing Techniques: Edge Detection and Frequency Analysis

<p align="center"> <img src="https://github.com/user-attachments/assets/6a0ac76d-8aba-4f11-af03-7c4764e37f4c" alt="Image Processing Example" width="600"> </p>

## 🚀 Overview
This project demonstrates fundamental **image processing techniques** using Python, including **Sobel edge detection**, **Gaussian blur**, **Laplacian filters**, and **Gabor filters**. These operations help detect edges, enhance features, and analyze textures in images.

> **Goal:** To visualize and explore different ways of identifying edges and frequency components in images.

---

## 🛠️ Features
- **Sobel X and Y Edge Detection**: Highlights vertical and horizontal edges.
- **Gaussian Blur**: Reduces noise and smooths the image.
- **Combined Sobel Edge Detection**: Detects edges in multiple directions.
- **Laplacian Edge Detection**: Identifies changes in intensity.
- **Gabor Filters**: Extracts textures with orientation-specific kernels.
- **Magnitude Spectrum Analysis**: Reveals the frequency domain of the image.

---

## 📂 Structure
```
CV Lab .ipynb
├── Image Reading and Preprocessing
├── Sobel X Edge Detection
├── Sobel Y Edge Detection
├── Combined Sobel Detection
├── Gaussian Blur and Noise Reduction
├── Laplacian Edge Detection
├── Gabor Filters for Texture Detection
└── Magnitude Spectrum Transformation
```

---

## 🔧 Setup and Installation
Ensure you have Python and the required libraries installed:

```bash
pip install opencv-python-headless matplotlib numpy
```

---

## 📸 Sample Usage

```python
import cv2
import matplotlib.pyplot as plt

# Load and preprocess the image
image = cv2.imread('edge1.jpg', cv2.IMREAD_GRAYSCALE)
blurred = cv2.GaussianBlur(image, (5, 5), 0)

# Perform Sobel Edge Detection
sobel_x = cv2.Sobel(blurred, cv2.CV_64F, 1, 0, ksize=5)
sobel_y = cv2.Sobel(blurred, cv2.CV_64F, 0, 1, ksize=5)

# Display results
plt.subplot(1, 2, 1), plt.imshow(sobel_x, cmap='gray')
plt.title('Sobel X'), plt.axis('off')
plt.subplot(1, 2, 2), plt.imshow(sobel_y, cmap='gray')
plt.title('Sobel Y'), plt.axis('off')
plt.show()
```

---

## 📊 Results

Below are examples of the outputs from different techniques:

Sobel X and Y Edge Detection
<p align="center"> <img src="https://github.com/user-attachments/assets/8746b615-9b59-40bb-a6f3-1777a5fb72d4" alt="Sobel Edge Detection" width="600"> </p>
Gaussian Blur and Laplacian Edge Detection
<p align="center"> <img src="https://github.com/user-attachments/assets/44d5b67f-eada-4f4f-9c33-93f40be65ce0" alt="Laplacian Edge Detection" width="600"> </p>

## 🎨 Visualization
The notebook also visualizes the **magnitude spectrum** and **Gabor-filtered textures**, showcasing how frequency analysis helps reveal underlying patterns in images.

---

## 🤖 Technologies Used


![Python](https://img.shields.io/badge/Python-3.x-blue)
![OpenCV](https://img.shields.io/badge/OpenCV-4.8-green)
![License](https://img.shields.io/badge/License-MIT-orange)

- **Python**: Core programming language  
- **OpenCV**: Image processing library  
- **NumPy**: Numerical operations  
- **Matplotlib**: Visualization tool  

---

## 📝 License :
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💬 Contact
For any questions, feel free to reach out:  
**Prajwal Koundinya**  
📧 prajwalkowndinya@gmail.com  

---

## ⭐ Acknowledgments
- Thanks to **OpenCV** and **Python** communities for excellent documentation and support.  

---
