# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import opencv.

### Step2:
Read the original Image.

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program.

## Program:
```
# Developed By: JAYASRI DODDA
# Register Number: 212222240028
```
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('EXXX3.jpeg')
cv2.imshow('Original Image',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

# ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('EXXXX3.jpeg')
cv2.imshow('Original HSV Image',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('EXXXX3.jpeg')
cv2.imshow('Original HSV Image',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('EXXXX3.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('EXXXX3.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow

```

## Output:

### i) BGR and RGB to HSV and GRAY
![1](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/1b6fbf53-8285-491e-8ba3-879abab91751)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/acf14b60-2c2d-4a9e-9b29-a88e4b8c4987)
![3](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/fc5b65b7-8efc-40f4-bde4-b2a18ed14a68)
![4](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/9de84520-2d6b-426d-a768-76712a10076f)
![5](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/5eb83c16-7e93-4792-9842-755f445cfd99)
![6](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/2749a81f-005b-45be-8f6a-a5119ef32ccd)

### ii) HSV to RGB and BGR
![1](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/3f6483a8-748d-424e-9435-732e6c71862e)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/c7fc478b-79c9-4e84-8feb-568f639c1a19)
![3](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/530743bf-45fc-41bb-b816-bf1cee5e28da)
![4](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/e6efa532-bbef-4c94-985f-f1516a12c5b9)

### iii) RGB and BGR to YCrCb
![1](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/51d487a1-0b31-4602-b38c-301f2a846b70)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/4ca41146-bb0d-45ec-bab4-bbc1a4a9ea75)
![3](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/35262051-d9ed-427d-8017-41be3120521d)
![4](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/d6a8130d-8f7e-4144-8c88-98fc70f951a2)

### iv) Split and merge RGB Image
![1](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/d0b78a70-c3aa-4167-a65b-71631eaca203)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/d202edb1-a9e9-438f-8420-9657458e67a9)
![3](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/95eaceb8-78cb-4640-a757-32fd502db0b5)
![4](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/6016868a-8e15-411d-8c53-be716f2dc0fa)
![5](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/1ee86bfa-bf93-42f8-9152-e0ecc178c765)


### v) Split and merge HSV Image
![1](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/f55b2040-fcc4-460b-a3ed-6400b98b7f6c)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/88b012d5-6c40-4ac4-83ec-64909022e499)
![3](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/527dd1a1-4010-4c03-9a30-d84e4f6f25b7)
![2](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/32e6eb31-d546-4e41-8e50-bd48b88c997b)
![4](https://github.com/jayasridodda/COLOR-CONVERSION/assets/123259278/a6bf4f57-2a16-467e-9390-10bb6ff151f6)


## Result:

Thus the color conversion was performed between RGB, HSV and YCbCr color models.
