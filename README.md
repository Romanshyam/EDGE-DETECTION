# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.
### Step2:
Load a image using imread() from cv2 module.
### Step3:
Convert the image to grayscale
### Step4:
Using Sobel operator from cv2,detect the edges of the image.
### Step5:
Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.
## PROGRAM:
```
 DEVELOPED BY: Shyam Kumar E
 REGISTER NUMBER: 212223230207
```
## IMPORT PACKAGES AND LOAD IMAGES
  ```python
import cv2
import matplotlib.pyplot as plt

img=cv2.imread("aizen.jpg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
## SOBEL EDGE DETECTOR:
## SOBEL X:
  ```python
  sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
## SOBEL Y:
```python
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.imshow(sobely,cmap='gray')
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
## SOBEL XY:
  ```python
  sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
## LAPLACIAN EDGE DETECTOR:
```python
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
## CANNY EDGE DETECTOR:
```python
canny=cv2.Canny(gray,120,150)
plt.imshow(canny,cmap='gray')
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
## ORIGINAL IMAGE:
![aizen](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/9d42817a-f04c-402a-b1ef-f0d7fac364a9)

### SOBEL EDGE DETECTOR:
![Screenshot 2024-04-10 102250](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/db0e4f57-b070-4908-a2d7-ba336b13992e)

![Screenshot 2024-04-10 102358](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/84b3d7c3-8625-40c3-aab9-b4b7caf9d1ac)

![Screenshot 2024-04-10 102317](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/63a99d9d-f92c-469b-a32b-739c396a89ef)

### LAPLACIAN EDGE DETECTOR
![Screenshot 2024-04-10 102427](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/af6bdd50-4583-4db1-8ee0-8c1481681500)

### CANNY EDGE DETECTOR
![Screenshot 2024-04-10 102449](https://github.com/KameshLeVI/EDGE-DETECTION/assets/120780633/a37c24c8-ca84-423d-be53-0bb613df8e97)


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
