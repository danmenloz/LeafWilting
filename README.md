# ECE 542 | Team 21 | Project 1.2: Leaf Wilting Detection in Soybean
This is a nerual networks project that aims to rate images from a scale of 0 (No wilting) to 4 (Severe turgor loss throughout canopy).

## How to run this project?
There are 3 main files: *Dataset.ipyb*, *VGG16.ipynb* and *Results.ipynb*. The */TrainingData* directory holds the training images and their annotations in a CSV file, and th */prediction* directory holds the images whose labels have to be predicted.

Follow the next steps to generate the predicitions:

1. Download the files and copy them into your Google Drive root folder under the directory name *ECE_542-Project1*. Your Google Drive should look as follows:
    * My Drive/ECE_542-Project1/prediction/...  
    * My Drive/ECE_542-Project1/TrainingData/...  
    * My Drive/ECE_542-Project1/VGG16.ipynb  
    * My Drive/ECE_542-Project1/Dataset.ipyb  
    * My Drive/ECE_542-Project1/Results.ipynb  
  
2. First, create the dataset structure. To do this, run *Dataset.ipyb*. This script will organize the images in */TrainingData* according to their label. After running this script, you should get the following directory structure with images in there:
    * My Drive/ECE_542-Project1/data/validation
    * My Drive/ECE_542-Project1/data/validation/0
    * My Drive/ECE_542-Project1/data/validation/1
    * My Drive/ECE_542-Project1/data/validation/2
    * My Drive/ECE_542-Project1/data/validation/3
    * My Drive/ECE_542-Project1/data/validation/4
    * My Drive/ECE_542-Project1/data/train
    * My Drive/ECE_542-Project1/data/train/0
    * My Drive/ECE_542-Project1/data/train/1
    * My Drive/ECE_542-Project1/data/train/2
    * My Drive/ECE_542-Project1/data/train/3
    * My Drive/ECE_542-Project1/data/train/4      
    * My Drive/ECE_542-Project1/data/test
    * My Drive/ECE_542-Project1/data/test/0
    * My Drive/ECE_542-Project1/data/test/1
    * My Drive/ECE_542-Project1/data/test/2
    * My Drive/ECE_542-Project1/data/test/3
    * My Drive/ECE_542-Project1/data/test/4    

3. Next, run *VGG16.ipynb*. This will create a Neural network model and will train using the created dataset. Training will take about 15 min and the result will be stored in the next *.h5* file:
    * My Drive/ECE_542-Project1/vgg16_model.h5
  
4. Finally, run *Results.ipynb* to generate a prediction which will be stored in the next CSV file:
    * My Drive/ECE_542-Project1/predictions.csv
  
