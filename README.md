# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:shaik sameer
### Register Number: 21221240051
i) #To Read,display the image
```
 import cv2
color_img=cv2.imread('mom.png',1)
cv2.imshow('212221240051,S.sameer',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
color_img = cv2.imread('mom.png',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('212221240051-s.sameer',color_img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```python3

import cv2
colorImage = cv2.imread('mom.png',1)
print(colorImage.shape)

```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('mom.png',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240051,S.sameer',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python3
import cv2
color_img=cv2.imread('mom.png',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221240051,S.sameer',color_img)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


