# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
<br>

i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.
<br>
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
### Developed By: Vishranthi A
### Register Number: 212221230124
i) #To Read,display the image
```
import cv2
color= cv2.imread('flower.png',1)
cv2.imshow('212221230124 VISHRANTHI A',color)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
color= cv2.imread('flower.png',1)
cv2.imwrite('VISHRANTHI A.png',color)
```
iii) #Find the shape of the Image
```
import cv2
color= cv2.imread('flower.png',1)
print(color.shape)
```
iv) #To access rows and columns

```
import cv2
import random
color= cv2.imread('flower.png',1)
for i in range(100):
    for j in range(color.shape[1]):
        color[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230124 VISHRANTHI A',color)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color= cv2.imread('flower.png',1)
tag=color[200:300,200:300]
color[100:200,100:200]=tag
cv2.imshow('212221230124 VISHRANTHI A',color)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image
![1](https://user-images.githubusercontent.com/93427278/225696845-142748d3-978e-488e-a396-88c27999ab00.png)

### ii)Write the image
![2](https://user-images.githubusercontent.com/93427278/225696874-e595c18a-8785-47de-bd14-c41b4bd62be0.png)

### iii)Shape of the Image
![3](https://user-images.githubusercontent.com/93427278/225696921-1af7a038-03cc-4b6d-8147-e085df8b8daa.png)

### iv)Access rows and columns
![4](https://user-images.githubusercontent.com/93427278/225696986-9864a3ef-78c6-4252-b195-3cb181539c98.png)

### v)Cut and paste portion of image
![5](https://user-images.githubusercontent.com/93427278/225697019-ff35aeaf-c2ea-416f-9e79-646fbd1f2641.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


