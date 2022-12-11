
## Folder Name : Saving Grapheme Images from BengaliAI
## File Name : GraphemeimgSaving.ipynb


## Necessary Imports : PIL,json,cv2,os,glob,pickle,pandas,numpy,pyarrow
## for installing pyarrow : conda install -c conda-forge pyarrow   OR   pip install pyarrow
## for installing pandas : pip install pandas
## for installing numpy : pip install numpy

## How to run the Code :
1) Install all the dependencies
2) Download the dataset from here : https://www.kaggle.com/c/bengaliai-cv19/data
3) set all the paths of csv and perquet accordingly in the code.
4) Create a destination folder for grapheme image to save and set the path in code.
5) Run the code.


## Description:
From the Step 1 we got three pickle files. in this section our objective is to save grapheme images from the bengali AI dataset. for this we used those pickle files. before that, Bengali AI dataset contains a csv file("Train.csv") 
and parquet files (Which contained images). both files had a common id. using this ID we could link up both files and save images from perquet file and label the image using the labels from csv files. but we do not need all the
images from the perquet file. we only needed the images we had in our grapheme image files as we only need those characters to construct words. so we loaded our grapheme dictionary here and searched all those characters
 from the train csv file and saved images according to grapheme dictionary . we saved images and labeled it with proper labels of the grapheme dictionary numbers so that in future we could search the image by the grapheme 
dictionary number. 