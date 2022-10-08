# Plankton-Image-Classification

## Aim
The Aim is to solve the following classification problem:

The dataset contains 31 classes of plankton images captured using CytoSense during 2020 and annotated by biologists from the Finnish Environment Institute (SYKE) in February 2021

## DATA

- The path to the dataset needs to be changed in the code.
- The dataPath variable should point to the root folder of the dataset.
- The preprocessing will create two folders inside the dataset root folder, where the processed images are saved

## EXECUTING THE CODE

- Example run of all the functions are in main.m file. 
- densenet_test.m can be run individually to test the pre-trained network.

## NOTES
The CNN training follows the MATLAB [GoogLeNet example](https://se.mathworks.com/help/releases/R2019b/deeplearning/examples/train-deep-learning-network-to-classify-new-images.html).

FreezeWeights.m, findLayersToReplace.m and createLgraphUsingConnections.m are from the same example.
