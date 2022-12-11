## Folder Name : All Images Cropping and Saving in a single Folder
## File Name : CroppedinaSingleFolder.ipynb



## Necessary Imports : PIL,Json,cv2, OS 
 ##for installing openCV use : pip install opencv-contrib-python


## How to run the file:
1) Install all the dependencies
2) Download the dataset : https://data.mendeley.com/datasets/r43wkvdk4w/1?fbclid=IwAR3-3Sw2rmKKxWVYQQIwlA7A40db3uvCt6jyFAwakXxPonk_Rm_Qc1Xdv88
3) Create a destination folder where you want your image to be saved.
4) Fix the filepath locations in the code.


##Description:
In this code we extended our previous work. this time we took all the images from the given dataset in a loop and also all the json files values through a loop and cropped every word 
according to its bounding points and also renamed the images with the given labels in the json file and saved the images. in this section we saved all words from different images in a single folder. 
We just unified them to get a bigger dataset.