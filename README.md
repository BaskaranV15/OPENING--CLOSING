# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Read the image
### Step3:
Create the structuring element or kernal element
### Step4:
Use Opening operation
### Step5:
Use Closing Operation
 
## Program:

``` Python
Import the necessary packages

import cv2
import numpy as np

Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,'THEBOSS',(5,35),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("212222230020_baskaran",img1)
cv2.waitKey()
cv2.destroyAllwindows()

# Create the structuring element
kernal=np.ones((5,5),np.uint8)


# Use Opening operation
mg1o=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernal)
cv2.imshow("baskaran_212222230020",img1o)
cv2.waitKey(0)
cv2.destroyAllwindows()


# Use Closing Operation
imglc=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernal)

cv2.imshow("baskaran_212222230020",imglc)
cv2.waitKey(0)
cv2.destroyAllwindows()


```
## Output:

### Display the input Image

![Screenshot from 2023-10-10 18-15-32](https://github.com/BaskaranV15/OPENING--CLOSING/assets/118703522/8ca1be96-3764-4931-9a55-03213b1fb770)


### Display the result of Opening

![asdfghj](https://github.com/BaskaranV15/OPENING--CLOSING/assets/118703522/c11e0fbb-27f3-48d8-965b-15403daed7be)


### Display the result of Closing

![Screenshot from 2023-10-10 18-02-51](https://github.com/BaskaranV15/OPENING--CLOSING/assets/118703522/4c9ee069-9c43-4288-b816-7b97bbc08729)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
