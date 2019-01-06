# Histopathologic Cancer Detector NASNet CNN



### CNN Architecture
The problem is binary classification of 96x96 RGB images.

A topless NASNet convolutional neural network was used as the base model. The output of said base model is passed through Global Max Pooling, Global Average Pooling and Flattened parallely then these outputs are concatenated. Further, the concatenated output is passed through a fully connected layer with dropout during training and finally, there is a single output neuron with sigmoid activation function.



### How to run it?

1. Split & Organise Data
   - Download dataset from Kaggle (https://www.kaggle.com/c/histopathologic-cancer-detection/data)
   - Unzip to main folder (train/, test/, train_labels.csv)
   - Run split_and_organize
   
2. Build and Train
   - Run build_and_train
   - Model which best performs will be saved on the main folder
   
3. Load and Predict
   - Run load_and_predict
   - Model will be loaded and the test set labels will be predicted
   - Kaggle submission file will be generated
