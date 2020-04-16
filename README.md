# Crack Detection Using Convolution Neural Networks(CNN)

## Description
This repository contains the code for crack detection in concrete surfaces.
It is a TensorFlow implementation of Deep Learning-Based Crack Damage Detection
Using Convolutional Neural Networks.

MATLAB was used to prepare the data. Regions of Interest were sliced
into smaller 128 x 128 pixel images and used for training

## Requirments:

1. Tensor Flow

2. OpenCV

3. Dataset:  [Link](https://drive.google.com/file/d/1kC60RGO3rcScVk7HY-s7tTMJeMbADfh1/view)

## Implementation: 

To train the network run the command with followoing arguments

    Train_CD.py
```
## Argument                   Details                                        Defau

--in_dir                   path to in_dir folder                             cracky 

--iter                     number of iterations to run the model for         1500 

--save_folder              Directory to save checkpoint                      CURRENT_DIR

```


After model has been trained, meta_files are saved into 'save_folder'. 
To test the model, run the command with the following arguments: 
```
   Running.py
```

```
## Argument                  Details                                        Default

--in_dir             director containing unlabeled test data         cracky_test 
--meta_file          MetaFile path                                   None(will throw error if not given)
--cp_dir             dir contatining checkpoint                      None(will throw error if not given)
--save_dir           dir to save output images                       CURRENT_DIR   
```
