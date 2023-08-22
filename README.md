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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('CJ7.jpg',1)
cv2.imshow('212222100035_PRAKASH',color_img)
cv2.waitKey(0)  


```
ii) #To write the image
```
import cv2
color_img=cv2.imread('CJ7.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212222100035_PRAKASH',color_img)
cv2.waitKey(0) 




```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('CJ7.jpg',1)
print(color_img.shape)



```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('CJ7.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222100035_PRAKASH',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('CJ7.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222100035_PRAKASH',color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

![image](https://github.com/Prakashmathi2004/READ-AND-WRITE-IMAGE/assets/118350045/eea8f2a1-8b41-4b90-8100-b3cec1ede07b)


### ii)Write the image

<img width="724" alt="image" src="https://github.com/Prakashmathi2004/READ-AND-WRITE-IMAGE/assets/118350045/8d36bc51-2618-477c-924d-0028c3a77be4">


### iii)Shape of the Image

<img width="294" alt="image" src="https://github.com/Prakashmathi2004/READ-AND-WRITE-IMAGE/assets/118350045/07f1f44b-048b-47b9-9bc9-ccb3f842b11d">


### iv)Access rows and columns
![image](https://github.com/Prakashmathi2004/READ-AND-WRITE-IMAGE/assets/118350045/c019bd9f-49bf-46f8-a7ec-2c230be12e8d)



### v)Cut and paste portion of image
![image](https://github.com/Prakashmathi2004/READ-AND-WRITE-IMAGE/assets/118350045/f901a664-3787-404b-b89b-e9de7b4ae095)



## Result:
Thus the images are read, displayed, and written successfully using the python program.
