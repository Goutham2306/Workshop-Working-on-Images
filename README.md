# Workshop-Working-on-Images
## AIM :
The image should be converted to gray scale and HSV and display the H, S and V planes.

# Software Required :
jupyter Notebook

# Algorithm :
# Step1:
Choose an image , the image should be a plant , Tree, flower or building.

# Step 2:
Save the image and the filename should be username.jpg

# Step 3:
Convert the image to gray scale and HSV

# Step 4:
Display the H,S and V planes.

## Program :
# Developed By : Goutham.K
# Register Number : 212223110019
```
import cv2
import numpy as np
username = "Goutham"
image = cv2.imread("goutham.jpg")
image = cv2.resize(image,(300,200))
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
h, s, v = cv2.split(hsv)
cv2.imshow("Hue (H)", h)
cv2.imshow("Saturation (S)", s)
cv2.imshow("Value (V)", v)
cv2.imwrite(f"{username}_gray.jpg", gray)
cv2.imwrite(f"{username}_hsv.jpg", hsv)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## OUTPUT:
![image](https://github.com/Goutham2306/Workshop-Working-on-Images/assets/138971154/e5a5c02d-89af-42d0-a2c1-cffa39cbcf0a)

![image](https://github.com/Goutham2306/Workshop-Working-on-Images/assets/138971154/54445d11-aaea-478f-9241-d524f403116e)

![image](https://github.com/Goutham2306/Workshop-Working-on-Images/assets/138971154/a06a7334-3e94-4191-8288-226388dbbb64)

## RESULT:
   Thus the image is converted to gray scale and HSV using python and displayed successfully.
