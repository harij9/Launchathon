# Launchathon
UCB - 


Dependencies required-

TensorFlow
OpenCV
Dataset 

The dataset.py file creates the training dataset class to be fed into the Convolutional Neural Network. This class automatically determines the number of classes by the number of folders in 'in_dir' (number of folders=number of classes)

NOTE: This script utilizes an already saved cache file. The cache file contains the filenames of the data. If the cache file doesn't exist, a new one created. If the data has been altered with, please delete the old cache file and run the script again. This applies for both Running.py and Train_CD.py. 

The directory structure is assumed to be the following- (For example considering 3 classes)

in_dir/class1/ - Contains all the training images for class 1
test/ - Contains all the validation images for class 1 
in_dir/class2/ - Contains all the training images for class 2
test/ - Contains all the validation images for class 2
in_dir/class3/ - Contains all the training images for class 3
test/ - Contains all the validation images for class 3
To train the network run the command with the following arguments:
python Train_CD.py

Argument	Details	Default
--in_dir	path to in_dir folder	cracky
--iter	number of iterations to run the model for	1500
--save_folder	Directory to save checkpoint	CURRENT_DIR
After model has been trained, meta_files are saved into 'save_folder'. To test the model, run the command with the following arguments: python Running.py
