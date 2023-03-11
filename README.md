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
### Developed By: Y Shavedha
### Register Number: 212221230095
## Program:

i) #To Read,display the image
```
import cv2
colorimg=cv2.imread('spup2.jpg',1)
cv2.imshow('spup2',colorimg)
cv2.waitKey(0)  
```
ii) #To write the image
```
import cv2
colorimg = cv2.imread('spup2.jpg',1)
s = cv2.imwrite('spup2.jpg',colorimg)
cv2.imshow('shavs',colorimg)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
colorimg = cv2.imread('spup2.jpg',1)
print(colorimg.shape)
```
iv) #To access rows and columns

```
import random
import cv2
colorimg = cv2.imread('spup2.jpg',1)
for i in range(100):
    for j in range(colorimg.shape[1]):
        colorimg[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('spup2.jpg',colorimg)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
colorimg = cv2.imread('spup2.jpg',1)
tag = colorimg[300:400,300:400]
colorimg[50:150,50:150] = tag
cv2.imshow("shavs",colorimg)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
<img width="883" alt="1rw" src="https://user-images.githubusercontent.com/93427376/224496245-cfa9a12b-0558-4587-a7ab-b481f5bb2f1b.png">

### ii)Write the image
<img width="908" alt="2write" src="https://user-images.githubusercontent.com/93427376/224496262-17b326b9-0d53-4766-9d6c-752e0dd0988a.png">

### iii)Shape of the Image
<img width="494" alt="3shape" src="https://user-images.githubusercontent.com/93427376/224496298-bc886272-4bb0-4637-b79a-5cd589d5bf28.png">

### iv)Access rows and columns
<img width="929" alt="4rowsndco" src="https://user-images.githubusercontent.com/93427376/224496316-4c66eb06-ca0b-4f47-9af5-0afc76d4b96b.png">

### v)Cut and paste portion of image
<img width="883" alt="5cut" src="https://user-images.githubusercontent.com/93427376/224496341-27e335db-0fb0-4778-a166-f0b53ec9dc32.png">

## Result:
Thus the images are read, displayed, and written successfully using the python program.


