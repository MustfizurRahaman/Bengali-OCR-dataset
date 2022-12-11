## Folder Name : Generating Labels and graphemes from word dictionary
## File Name : Grapheme_worddict_labels_generator.ipynb

## Necessary Imports : PIL,json,cv2,os,glob,pickle,pandas,numpy,pyarrow
## for installing pyarrow : conda install -c conda-forge pyarrow   OR   pip install pyarrow
## for installing pandas : pip install pandas
## for installing numpy : pip install numpy

## How to run the Code :
1)Install All the Dependencies
2) fix the path of word_dict.pkl so that it can be read.
3)Run the code. it will automatically generate other pickle files.


## Description :
 In this folder we created pickle files for Word dictionary, labels and Grapheme dictionary. initially we needed a word dictionary to do that. we used a dataset which contained almost 800000 images with printed words. 
the dataset was properly labeled. so for constructing a word dictionary we used this dataset, extracted the labels from there , inserted all those labels in a list and saved that list in a python pickle file called "word_dict.pkl".
the coding part of creating word dictionary from images and saving are commented in this file. as later part we no more needed the images anymore we could just use the pickle file. 

after that we used that word_dict file to generate a grapheme dictionary. we had a grapheme generation function from the baseline model. but we needed to modify that function according to our need. after modifying we 
got a grapheme dictionary and using that grapheme dictionary we got labels file. we inserted them seperately in different list and saved both list as different names such as "Grapheme_dict.pkl" and "Labels.pkl". these files
further used for future modifications.