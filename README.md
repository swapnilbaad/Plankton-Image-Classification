# Plankton-Image-Classification

## Aim
The Aim is to solve the following classification problem:

The dataset contains 31 classes of plankton images captured using CytoSense during 2020 and annotated by biologists from the Finnish Environment Institute (SYKE) in February 2021

## Data

- The path to the dataset needs to be changed in the code.
- The dataPath variable should point to the root folder of the dataset.
- The preprocessing will create two folders inside the dataset root folder, where the processed images are saved

## Sample of Pre-Processed Input Images
<img width="1097" alt="image" src="https://user-images.githubusercontent.com/48822463/194699937-285882ee-acc2-43fc-815b-dfc8c4845b18.png">

## Executing the code

- Example run of all the functions are in main.m file. 
- densenet_test.m can be run individually to test the pre-trained network.

## Results
The model has an accuracy of **80.99%** according to the testing with the test set. 
Below Figurea confusion matrix of the test run. Some plankton species share very similar characteristics with each other, for example the Cryptomonadales and the Cryptophyceae-Teleaulax are very similar. That also shows on the confusion matrix, since nearly half of the Cryptomonadales have been misclassified as the Cryptophyceae-Teleaulax.
![confusion_matrix](https://user-images.githubusercontent.com/48822463/194699737-c5dffa39-1024-41c2-bf33-cbade40d7c06.png)

## Notes
The CNN training follows the MATLAB [GoogLeNet example](https://se.mathworks.com/help/releases/R2019b/deeplearning/examples/train-deep-learning-network-to-classify-new-images.html).

FreezeWeights.m, findLayersToReplace.m and createLgraphUsingConnections.m are from the same example.
