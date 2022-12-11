## Folder Name : constructing words using grapheme images
## File Name : Cropped_concatanated_imgdict_Generator.ipynb


## Necessary Imports : PIL,json,cv2,os,glob,pickle,pandas,numpy,pyarrow
## for installing pyarrow : conda install -c conda-forge pyarrow   OR   pip install pyarrow
## for installing pandas : pip install pandas
## for installing numpy : pip install numpy

## How to run the Code : 
1) Install all the dependencies 
2) Set all the paths correctly( load pickle files, Set path of Grapheme img folder)
3) Create a destination folder where you want to save your images. and set the path file correctly
4) Run the Code

## Description:
In this coding file our objective was to construct words using the grapheme images we got from the last section. for doing this we loaded all the three pickle files we got in the first section. also we loaded our
grapheme image directory which we saved in the last section. after that we create a loop and extract grapheme from every word and search that graphemes image from our specified folder. If we are able to match all the images
from our folder we then horizontally concatenate it and rename the new image as the word name and save it in a specific folder. If we fail to search for one or two words from the grapheme image folder we just skip that word from
concatenating. by doing this all the images we are saving are valid and ready to use.

but after doing that the problem arised that all the characters were very much distanced from each other. so our next objective was to reduce this distance. to solve this problem we modified our code. before concatenating
the character images we searched for the contour points for every character and cropped the images before concatanating those. by doing this the distance between those characters were removed and our problem was solved.