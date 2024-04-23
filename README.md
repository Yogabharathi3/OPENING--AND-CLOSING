## OPENING--AND-CLOSING
### Aim
To implement Opening and Closing using Python and OpenCV.

### Software Required
1. Anaconda - Python 3.7
2. OpenCV
### Algorithm:
#### Step1:
Import the necessary packages
#### Step2:
Create the Text using cv2.putText
#### Step3:
Create the structuring element
#### Step4:
Use Opening operation
#### Step5:
Use Closing Operation

### Program:
```
Developed by: Yogabharathi
Register Number:212222230179
```
## Import the necessary packages :
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
## Create the Text using cv2.putText :
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'ABRIN NISHA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
## Create the structuring element :
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
## Use Opening operation :
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
## Use Closing Operation :
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```
### Output:

#### Display the input Image
![image](https://github.com/Yogabharathi3/OPENING--AND-CLOSING/assets/118899387/7b706892-1688-4d1a-9446-b63d605e1448)

#### Display the result of Opening
![image](https://github.com/Yogabharathi3/OPENING--AND-CLOSING/assets/118899387/0e1529bb-ba6e-404f-b0ce-b564f4f7f85a)

#### Display the result of Closing
![image](https://github.com/Yogabharathi3/OPENING--AND-CLOSING/assets/118899387/f92a05e0-c9bf-48f0-b87b-8019933044b3)


### Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
