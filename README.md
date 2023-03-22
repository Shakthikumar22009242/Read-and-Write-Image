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

### Developed By: Shakthi kumar S
### Register Number: 212222110043
i) #To Read,display the image
```python
import cv2
color_img=cv2.imread('DIP 01.jpg',1)
cv2.imshow('DIP 01',color_img)
cv2.waiKey(0)
```
ii) #To write the image
```python
import cv2
color_img=cv2.imread('DIP 01.jpg',1)
a=cv2.imwrite('1.jpg',color_img)
cv2.imshow('DIP 01',color_img)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```python
import cv2
colorimage=cv2.imread('DIP 01.jpg',1)
print(colorimage.shape)
```
iv) #To access rows and columns

```python
import cv2
import random
color_img=cv2.imread('DIP 01.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('DIP 01',color_img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```python
import cv2
color_img=cv2.imread('DIP 01.jpg',1)
b=color_img[30:80,30:80]
color_img[100:150,100:150]=b
cv2.imshow('DIP 01',color_img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![](DIP%201-1.jpg)

### ii)Write the image

![](DIP%201-2.png)

### iii)Shape of the Image

![](DIP%201-3.png)

### iv)Access rows and columns
![](DIP%201-4.png)

### v)Cut and paste portion of image
![](DIP%201-5.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


