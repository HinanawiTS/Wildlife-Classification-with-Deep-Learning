# ECE228-project, Team 13: Wild Life Classification with Deep Learning Methods
This is the project repository for Group 13, Wildlife Classification with Deep Learning Methods.

Please download the data set from https://www.kaggle.com/datasets/iamsouravbanerjee/animal-image-dataset-90-different-animals and extract the data directly
in the directory of this repository.

This repository contains a data set that is augmented by our team (Augmented.zip). Please use git lfs service to pull them to the local as this is a relatively large data set.

### Project Team Members:
- Yiheng Ye, yiy291@ucsd.edu
- Andy Liu, anl043@ucsd.edu
- Zhexu Li, zhl411@ucsd.edu

### Requirements:
- python 3.9
- pandas 1.3.4
- numpy 1.21.4
- matplotlib 3.5.0
- PyTorch 1.11
- tqdm 4.64.0
- seaborn 0.11.2

### Instruction of Notebooks
Please run all of our code in a cuda-enabled envirnoment since we are using GPU for computation.

- The MLP_model.ipynb serves a first try on classifying the images. To run the MLP_model.ipynb, save the data set downloaded from kaggle to the directory animals/animals so under this directory we have 90 sub-directories for our different animals.

- The Project.ipynb is where our most of models and experiments ran. Please extract the Augmented.zip to get the augmented data set and change the data root in the notebook (under "Load Dataset" module) so the root is point to your extracted data set under which has sub-directories for different animals.