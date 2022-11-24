# Gender-Classification
## Algorithm

1.Install deepface

2.Import necessary packages

3.Read the image

4.Analyze the gender using deepface
Program:

/*
Program to implement 
Developed by   :DurgaDevi P
RegisterNumber :  212220230015
*/

#install deepface
pip install deepface

#import packages
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt

#read the image
img=cv2.imread('durga2.jpeg')
plt.imshow(img[:,:,::-1])
plt.show()

#Analyze gender
result=DeepFace.analyze(img,actions=['gender'])
result2=DeepFace.analyze(img,actions=['emotion'])

#print the gender
print("Gender : ",result['gender'])

OUTPUT:

    CODE :

v2

    DEMO VIDEO YOUTUBE LINK:

https://youtu.be/yFzrwsKESZg
