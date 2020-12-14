# Fire Detection Net
This notebook was used in making a binary classifier for classifying fire and non fire images.
The architecture used here is DenseNet available pretrained on imageNet at keras application module. The dataset contained 10k images with 6k non fire images and 4k fire images.
The dataset was obtained from kaggle and google images. 

# Preprocessing
The preprocessing was done using openCV which was used to resize the images to 224x224 image size
SKlearn train test split was used to split the data into train and validation set 
ImageDataGenerator from Kaggle was used for data augmentation as well feeding batches to the model.

# Architechture 
The densenet121 model pretrained on imagenet was downloaded via the keras Application module.
75% of the model was frozen and 25% of the model was unfrozen and used in training. Two small 
fully connected layer with 8 and 1 unit were added after the model and  the final year had a 
sigmoid.

# Optimizer and loss function
Adam optimizer and binary cross entropy loss function was used.

