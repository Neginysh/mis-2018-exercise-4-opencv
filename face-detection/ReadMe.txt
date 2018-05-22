Project procedure:

1. First step is face detection which is mostly taken from:
https://github.com/opencv/opencv/tree/master/samples/android/face-detection

2. The position of detected faces are then stored is an array of rectangles.

3. The rectangles are stored in a Mat object

3. Nose detection is done on each face which is converted to Mat object. The .xml nose classifier is taken from :
http://www.technolabsz.com/2012/03/opencv-facenosemoutheye-concurrent.html

4. For putting a red circle on noses on original image the center of nose is found and then it is added to the top left corner of the face rectangle in the original image

5. The radius of the red circle is the height of detected nose rectangle divided by 2. 
 

