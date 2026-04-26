# Image Edge Detection Using Gradient (Vector Calculus Approach)

## Overview
This project applies vector calculus (gradient) to detect edges in images. The image is modeled as a scalar field I(x, y), and edges are identified where intensity changes sharply.

## Objective
Detect edges by computing the gradient magnitude of pixel intensity and extracting regions with high variation.

## Mathematical Formulation

Scalar field:  
I(x, y)

Gradient:  
∇I = ( ∂I/∂x , ∂I/∂y )

Gradient Magnitude (Main Formula):  
|∇I| = sqrt( (∂I/∂x)^2 + (∂I/∂y)^2 )

Interpretation:
- High |∇I| → edges  
- Low |∇I| → smooth regions  

## Working Principle

The image is treated as a scalar field I(x, y).  
Partial derivatives measure intensity change:

- ∂I/∂x → horizontal change  
- ∂I/∂y → vertical change  

These are computed using the Sobel operator.  
The gradient magnitude determines edge strength.

## Methodology

1. Load input image  
2. Convert to grayscale  
3. Compute gradients using Sobel operator  
4. Calculate gradient magnitude  
5. Normalize values  
6. Apply threshold  
7. Display results  

## Technologies Used

- Python  
- OpenCV  
- NumPy  
- Matplotlib  

## Input and Output

Input Image:  
![Input](images/input.jpg)

Output Image (Edge Detection):  
![Output](images/Output.png)

## How to Run

Step 1: Install Dependencies  
pip install opencv-python numpy matplotlib  

Step 2: Run Project  
jupyter notebook  

Open:  
vector.project.ipynb  

Run all cells to see output.

## Results

- Original image  
- Gradient magnitude image  
- Edge detection result  

## Applications

- Object detection  
- Medical imaging  
- Autonomous systems  
- Image segmentation  
- Computer vision  

## Conclusion

This project shows how vector calculus (gradients) can be applied to image processing.  
Gradient magnitude effectively detects edges by identifying intensity variations.
