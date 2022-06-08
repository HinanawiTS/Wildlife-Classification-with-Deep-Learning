# ECE228-project, Team 13: Wild Life Classification with Deep Learning Methods
This is the project repository for Group 13, Wildlife Classification with Deep Learning Methods.

Please download the data set from https://www.kaggle.com/datasets/iamsouravbanerjee/animal-image-dataset-90-different-animals and extract the data directly
in the directory of this repository.

This project requires a data set that is augmented from the previous data set by our team (processed.zip). Please use the link provided in the "Instruction of Notebooks" section to download it to the local as this is a relatively large data set. Please extract the data directly in the directory of this repository.

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

- The MLP_model.ipynb serves a first try on classifying the images. To run the MLP_model.ipynb, download the data from the kaggle link and directly extract it to this directory. In this way, there will be a directory called animals shown and there will be sub-directories for different animals under the path animals/animals.
- Link to the augmented dataset (processed.zip): https://drive.google.com/file/d/1OBu5znTCq0wseK4oersFblD7RUCShLdF/view?usp=sharing. Please download it to this directory to run the notebook below.
- The Project.ipynb is where our most of models and experiments ran. Please extract the processed.zip to the root directory directly to get the augmented data set and change the data root in the notebook (under "Load Dataset" module) so the root is point to your extracted data set under which has sub-directories for different animals. (If you extract the data directly, the data root shoud be processed/processed, but you should also check if you have sub-directories under this path.)
