# WORKSHOP 3 : Canny-Edge-Detection
<H3>Name: PREETHI A K </H3>
<H3>Register no: 212223230156</H3>
<H3>Date: 09.11.2025 </H3>

# AIM:
To implement the Canny edge detection algorithm on a sample image to identify and extract the edges, and to study the effect of different parameter settings (thresholds and smoothing) on the detected edges.

# PROGRAM:
```

import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('image.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()

```

# OUTPUT:
## Original Image
<img width="381" height="511" alt="image" src="https://github.com/user-attachments/assets/c4975294-ecb3-4e0f-96b6-c5cf54eabefa" />


## Canny Edges 
<img width="397" height="511" alt="image" src="https://github.com/user-attachments/assets/d040e4f4-215f-4d0b-904d-812e9f3a40f1" />

