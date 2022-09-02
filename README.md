# Wildlife Classification with Deep Learning 
### Introduction
The effectiveness of wildlife preservation relies heavily on in-depth understandings of the diversity and behavior of animals, which requires intensive manual labor of experts to correctly label the images collected. In this project, we construct a robust deep learning model to automate this process, through transfer learning with various state-of-the-art deep learning architectures, and improving network structures to better fit our tasks. We experimented with a number of state-of-the-art deep learning models, benchmarked their performance, and improved upon the best performing network. Trained on a heavily augmented dataset of animals, our improved ResNet50 model achieved a test accuracy of 93% which is 7% higher than the vanilla ResNet50 model, and our improved Wide-Resnet50 model achieved an impressive test accuracy of 96.2%, which introduced over 5% improvement over the vanilla Wide-ResNet model, with a little extra computational cost. 

Please be aware that this project was developed in collaboration with two teams from two classes (which was approved by instructors in both classes), one team focused on benchmarking different networks, improving the ResNet network, and analyzing the performance gains, while the other team focused on data augmentation, improving the WideResNet network, and visualizing the decision making process of the network. My contribution includes: experimented and benchmarked all models used in the project (except MLP), developed the "Regularization block" which led to the improvement in performance, analyzed and visualized the improvement analysis, implemented CAM for visualization of the network, wrote the reports, delivered the presentations, and effectively communicated between two teams. 

Please download the data set from https://www.kaggle.com/datasets/iamsouravbanerjee/animal-image-dataset-90-different-animals and extract the data directly
in the directory of this repository.

To achieve the a similar performance it's required to use a data set that is augmented from the previous data set by our team (processed.zip). Please use the link provided in the "Instruction of Notebooks" section to download it to the local as this is a relatively large data set. Please extract the data directly in the directory of this repository.

### Project Team Members:
- Zhexu Li, zhl411@ucsd.edu 
- Yiheng Ye, yiy291@ucsd.edu
- Andy Liu, anl043@ucsd.edu
- Juoyun Chen, juc026@ucsd.edu

### Instruction of Notebooks

Please run all of our code in a cuda-enabled envirnoment since we are using GPU for computation. 

- Link to the augmented dataset (processed.zip): https://drive.google.com/file/d/1OBu5znTCq0wseK4oersFblD7RUCShLdF/view?usp=sharing. Please download it to this directory to run the notebook below.
- The Resnet50 and Improvement Analysis.ipynb is for benchmarking different state-of-the-art models, improving the ResNet, and analyzing the performance gains. Please extract the processed.zip to the root directory directly to get the augmented data set and change the data root in the notebook (under "Load Dataset" module) so the root is point to your extracted data set under which has sub-directories for different animals. (If you extract the data directly, the data root shoud be processed/processed, but you should also check if you have sub-directories under this path). Report is Resnet50 and Improvement Analysis.pdf

- The WideResNet50 and CAM Visualization.ipynb is for data augmentation, improving the WideResNet, and visualizing the network using CAM (Class Actication Map). Report is WideResNet50 and CAM Visualization.pdf

- The MLP_model.ipynb serves a first try on classifying the images. To run the MLP_model.ipynb, download the data from the kaggle link and directly extract it to this directory. In this way, there will be a directory called animals shown and there will be sub-directories for different animals under the path animals/animals.

### Requirements:
- python 3.9
- pandas 1.3.4
- numpy 1.21.4
- matplotlib 3.5.0
- PyTorch 1.11
- tqdm 4.64.0
- seaborn 0.11.2
