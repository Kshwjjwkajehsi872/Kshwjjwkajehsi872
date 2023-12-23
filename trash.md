import cv2
from cvzone import HandTrackingmodule

cap=cv2.VideoCapture(0)
detector=HandTrackingmodule.HandDetector()

while(true)
succes.img=cap.read()
detector.findHands(img)
cv2.imshow('image',img)
cv2.waitkey(1)
