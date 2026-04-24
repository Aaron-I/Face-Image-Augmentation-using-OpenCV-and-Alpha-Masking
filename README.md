# Face-Image-Augmentation-using-OpenCV-and-Alpha-Masking

A simple project that adds sunglasses to a face image using alpha masking in OpenCV.

## Overview
1. Takes a face image
2. Places sunglasses on the eye region
3. Uses transparency (alpha channel) for smooth blending
## Tools Used
  1. Python
  2. OpenCV
  3. NumPy
  4. Matplotlib
## How it works
  1. Load face and sunglasses image
  2. Extract alpha channel as mask
  3. Resize images to match
  4. Blend using:
     ```
     maskedEye = eyeROI * (1 - mask)
     maskedGlass = glass * mask
     final = maskedEye + maskedGlass
     ```

## Output:
  
  <img width="1331" height="745" alt="image" src="https://github.com/user-attachments/assets/fb53d056-cebf-4177-83c3-dfb0ba9c7b69" />

## Acknowledgement

This project is inspired by basic computer vision and AR filter techniques used in modern applications like Snapchat and Instagram.
