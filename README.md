# Image Edge Detection Using Gradient (Vector Calculus Approach)

---

## 1. Overview

This project demonstrates edge detection in digital images using concepts from vector calculus. The image is modeled as a scalar field **I(x, y)**, and edges are identified based on variations in pixel intensity.

---

## 2. Objective

To detect edges in an image by computing the gradient magnitude of pixel intensity values and identifying regions with high spatial variation.

---

## 3. Mathematical Formulation

An image is represented as:

    I(x, y)

Gradient of the image:

    ∇I = ( ∂I/∂x , ∂I/∂y )

Gradient magnitude (edge strength):

    |∇I| = √( (∂I/∂x)²
              + (∂I/∂y)² )

Where:
- ∂I/∂x → change in intensity along horizontal direction  
- ∂I/∂y → change in intensity along vertical direction  

Interpretation:
- High |∇I| → Strong edges  
- Low |∇I| → Smooth regions  

---

## 4. Working Principle

The input image is treated as a scalar field where each pixel represents intensity.

1. Compute horizontal gradient (∂I/∂x)  
2. Compute vertical gradient (∂I/∂y)  
3. Combine both to calculate gradient magnitude  

    |∇I| = √( Ix² + Iy² )

The Sobel operator is used to approximate these derivatives.  
A threshold is then applied to extract only significant edges.

---

## 5. Methodology

1. Load input image  
2. Convert image to grayscale  
3. Compute gradients using Sobel operator  
4. Calculate gradient magnitude  
5. Normalize intensity values  
6. Apply thresholding  
7. Display results  

---

## 6. Technologies Used

- Python  
- OpenCV  
- NumPy  
- Matplotlib  

---

## 7. Input and Output

**Input Image**

![Input](images/input.jpg)

**Output Image (Edge Detection)**

![Output](images/Output.png)

---

## 8. How to Run

### Step 1: Install Dependencies

    pip install opencv-python numpy matplotlib

### Step 2: Launch Jupyter Notebook

    jupyter notebook

### Step 3: Run the Project

- Open file: `vector.project.ipynb`  
- Click **Run All Cells**  
- Output images will be displayed  

---

## 9. Results

The system generates:

- Original image  
- Gradient magnitude image  
- Final edge-detected output  

Edges are clearly visible in regions with high intensity variation.

---

## 10. Applications

- Object detection  
- Medical imaging (MRI, CT scans)  
- Autonomous navigation  
- Image segmentation  
- Computer vision systems  

---

## 11. Conclusion

This project demonstrates the practical application of vector calculus in image processing. By modeling an image as a scalar field and computing its gradient, edges can be effectively detected. This technique forms a fundamental component of modern computer vision and artificial intelligence systems.
