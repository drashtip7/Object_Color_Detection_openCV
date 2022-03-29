
Work Flow Description:
-----------------------
Performed steps 

 1: Input: Capture video through webcam.
 2: Read the video stream in image frames.
 3: Convert the imageFrame in BGR(RGB color space represented as three matrices of red, green and blue with integer values from 0 to 255) to HSV(hue-saturation-value) color space. Hue describes a color in terms of saturation, represents the amount of gray color in that color and value describes the brightness or intensity of the color. This can be represented as three matrices in the range of 0-179, 0-255 and 0-255 respectively.
 4: Define the range of each color and create the corresponding mask.
 5: Morphological Transform: Dilation, to remove noises from the images.
 6: bitwise_and between the image frame and mask is performed to specificaly detect that particular color and discrad others.
 7: Create contour for the individual colors to display the detected colored region distinguishly.
 8: Output: Detection of the colors in real-time.