### READ AND WRITE AN IMAGE
### AIM:
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

### Software Required:
Anaconda - Python 3.7

### Algorithm:

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
### Program:
### Developed By: Vishwa Rathinam S
### Register Number: 212221240063
i) #To Read,display the image
```
import cv2
A=cv2.imread("viswa.jpg",1)
cv2.imshow("212221240063",A)
cv2.waitKey(0)

```
ii) #To write the image
```
A=cv2.imread("viswa.jpg",1)
cv2.imwrite("outer1.png",A)
cv2.imshow("212221240063",A)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```
import cv2
pic = cv2.imread('viswa.jpg',3)
print(pic.shape)


```
iv) #To access rows and columns

```
import random
import cv2
A=cv2.imread("viswa.jpg",5)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221240063",A)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```

import cv2
A=cv2.imread("viswa.jpg",6)
tag=A[140:240,165:180]
A[25:125,50:65]=tag
cv2.imshow("212221240063",A)
cv2.waitKey(0)

```

### Output:

### i) Read and display the image
![Screenshot (23)](https://user-images.githubusercontent.com/95266350/225222877-ebec2764-c72e-4e62-83ba-bde71e0e2aa1.png)



### ii)Write the image
![Screenshot (23)](https://user-images.githubusercontent.com/95266350/225223023-3cfb4206-a011-4bd4-a733-ad80c583e74a.png)



### iii)Shape of the Image

![Screenshot (26)](https://user-images.githubusercontent.com/95266350/225223219-4d3993c2-7478-4035-b6ce-2a1eda33fdec.png)

### iv)Access rows and columns
![Screenshot (24)](https://user-images.githubusercontent.com/95266350/225223258-fedb638f-3144-40e4-8895-5768f169ebba.png)



### v)Cut and paste portion of image

![Screenshot (25)](https://user-images.githubusercontent.com/95266350/225223276-b51c0d58-0461-4105-87b9-816e8d0c55b8.png)

### Result:
Thus the images are read, displayed, and written successfully using the python program.


