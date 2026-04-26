# Image Edge Detection Using Gradient (Vector Calculus Approach)

## Overview
This project demonstrates edge detection in digital images using principles of vector calculus. The image is modeled as a scalar field I(x, y), and edges are detected by identifying regions with significant intensity variation.

## Objective
To detect edges in an image by computing the gradient magnitude of pixel intensity values and extracting regions with high spatial variation.

## Mathematical Formulation

An image is represented as a scalar field:

    I(x, y)

The gradient of the image is defined as:

    ∇I = ( ∂I/∂x , ∂I/∂y )

The gradient magnitude (edge strength) is given by:

    |∇I| = √ [ (∂I/∂x)² + (∂I/∂y)² ]

Where:
- ∂I/∂x represents intensity change along the horizontal direction  
- ∂I/∂y represents intensity change along the vertical direction  

Interpretation:
- High |∇I| → Strong edges  
- Low |∇I| → Smooth regions  

## Working Principle

The image is treated as a continuous scalar field. In practice, discrete approximations are used:

- Horizontal gradient (∂I/∂x) is computed using Sobel filter  
- Vertical gradient (∂I/∂y) is computed using Sobel filter  

The gradient magnitude is then calculated for each pixel. A threshold is applied to retain only significant intensity changes, resulting in the final edge-detected image.

## Methodology

1. Load the input image  
2. Convert the image to grayscale  
3. Compute horizontal and vertical gradients using Sobel operator  
4. Calculate gradient magnitude  
5. Normalize intensity values  
6. Apply thresholding  
7. Display results  

## Technologies Used

- Python  
- OpenCV  
- NumPy  
- Matplotlib  

## Input and Output

**Input Image**  
![Input](images/input.jpg)

**Output Image (Edge Detection)**  
![Output](images/Output.png)

## How to Run

Install required libraries:

    pip install opencv-python numpy matplotlib

Run the project:

    jupyter notebook

Open the file:

    vector.project.ipynb

Execute all cells to generate output.

## Results

The system produces:
- Original image  
- Gradient magnitude representation  
- Final edge-detected image  

Edges are clearly highlighted in regions with high intensity variation.

## Applications

- Object detection  
- Medical imaging (MRI, CT analysis)  
- Autonomous navigation systems  
- Image segmentation  
- Computer vision pipelines  

## Conclusion

This project demonstrates the practical application of vector calculus in image processing. By modeling an image as a scalar field and computing its gradient, edges can be effectively detected. This approach forms a fundamental component of modern computer vision systems.
