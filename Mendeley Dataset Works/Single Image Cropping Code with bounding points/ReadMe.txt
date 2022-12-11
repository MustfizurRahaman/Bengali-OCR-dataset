## Folder Name : Single Image Cropping Code with bounding points
## Code file names : 1) imgcrop.ipynb   2) singleImgCrop.ipynb

## Necessary Imports : PIL,Json,cv2, OS 
## for installing openCV use : pip install opencv-contrib-python

## How to run the file:
1) Install all the dependencies
2) Download the dataset : https://data.mendeley.com/datasets/r43wkvdk4w/1?fbclid=IwAR3-3Sw2rmKKxWVYQQIwlA7A40db3uvCt6jyFAwakXxPonk_Rm_Qc1Xdv88
3) Fix file path location in the code.


##Description:
## In these two folder the first one is mainly cropping a single word from a paragraph contained image. it takes four bounding points from the given Json file and then use those bounding points to crop the image only.

## the Second code is also doing the same thing but in this code it is extracting every values from the given json files and cropping every word the image contains. 