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
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: Janani.V.S
Register NO: 212222230050
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'JANANI.V.S', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

# Create the structuring element
struct_ele = np.ones((9, 9), np.uint8)

# Use Opening operation
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

# Use Closing Operation
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)

# Close all windows
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![image](https://github.com/janani225/OPENING--AND-CLOSING/assets/113497333/ddfaa374-8a10-4c5d-ab08-84a74b825a9b)


### Display the result of Opening
![image](https://github.com/janani225/OPENING--AND-CLOSING/assets/113497333/d143673c-1601-4cd5-af1b-3e777f433312)


### Display the result of Closing
![image](https://github.com/janani225/OPENING--AND-CLOSING/assets/113497333/ea2d9eaa-5891-4bac-924e-1524ec21f193)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
