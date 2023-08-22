# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
Step1: Choose an image and save it as a filename.jpg

Step2: Use imread(filename, flags) to read the file.

Step3: Use imshow(window_name, image) to display the image.

Step4: Use imwrite(filename, image) to write the image.

Step5: End the program and close the output image windows.:

## Program:
### Developed By:Goparapu Lutheesh
### Register Number:212221230029 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('1.jpg',1)
cv2.imshow('212221230029 Lutheesh',color_img)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
color_img=cv2.imread('1.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221230029 Lutheesh',color_img)
cv2.waitKey(0) 
```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('1.jpg',1)
print(color_img.shape)
```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('1.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230029 Lutheesh',color_img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('1.jpg',-1)
tag=color_image[30:40,30:40]
color_image[5:15,5:15]=tag
cv2.imshow('212221230029 Lutheesh',color_image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![WhatsApp Image 2023-08-22 at 21 20 24](https://github.com/Lutheeshgoparapu/READ-AND-WRITE-IMAGE/assets/94154531/936b87fa-014a-4d06-baca-41e2508da1e0)


### ii)Write the image

![WhatsApp Image 2023-08-22 at 21 20 24](https://github.com/Lutheeshgoparapu/READ-AND-WRITE-IMAGE/assets/94154531/8cec8761-940d-442d-8b3f-7391590c2709)


### iii)Shape of the Image
<img width="408" alt="262049934-db027aae-9652-4cf3-b964-069f428ca594" src="https://github.com/Lutheeshgoparapu/READ-AND-WRITE-IMAGE/assets/94154531/d39547f8-ad26-4cba-9d78-79db37abe723">



### iv)Access rows and columns


![WhatsApp Image 2023-08-22 at 21 20 24](https://github.com/Lutheeshgoparapu/READ-AND-WRITE-IMAGE/assets/94154531/d9a4bdd1-e770-48ba-9e9b-f8f7b15e98ac)


### v)Cut and paste portion of image

![WhatsApp Image 2023-08-22 at 21 20 24](https://github.com/Lutheeshgoparapu/READ-AND-WRITE-IMAGE/assets/94154531/3e7f821c-60d3-43e6-b0ca-f59873a47483)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
