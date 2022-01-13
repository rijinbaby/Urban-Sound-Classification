Name of the files: 
************************************************************************************************************************************************************
All the files follow this naming format.

"task_datasplit_NeuralNetwork_features_DataAugmentation"

for example:
usc_5050_DNN_mfcc_aug = UrbanSoundClassification, Using 5050 DataSplit for training and testing(as suggested), Using Deep Neural Network, Only MFCC fearures(40), With data Augmentation to increase the size of dataset 

usc_5050_DNN_mfcc      = UrbanSoundClassification, Using 5050 DataSplit for training and testing(as suggested), Using Deep Neural Network, Only MFCC fearures(40), No data Augmentation

usc_8020_CNN_all_aug = UrbanSoundClassification, Using 8020 DataSplit for training and testing, Using Convolutional Neural Network, MFCC and Other fearures, With data Augmentation to increase the size of dataset

************************************************************************************************************************************************************
Two Type of Neural Networks were used.

1. DNN  Deep Neural Network
2. CNN Convolutional Neural Network

************************************************************************************************************************************************************
Data Splits:
1.5050: Training = fold 1, 2, 3, 4, 6
	Testing= fold 5, 7, 8, 9, 10
2.8020: Training = fold 1, 2, 3, 4, 5, 6, 7, 8
	Testing= fold 9, 10
************************************************************************************************************************************************************
Features:
1. Only MFCC 
2. MFCC, chroma_stft, chroma_cens, rmse, zcr, mel, cent, rolloff, spec_bw, contrast, flatness
************************************************************************************************************************************************************
Augmentation:
Following data Augmentations were used.
1. Noise
2. Shift
3. Pitch
4. stretch

Using augmentaion increased the data size by 4x. 
************************************************************************************************************************************************************

Results: usc_8020_CNN_all_aug.ipynb shows the best results with 70% accuracy. 
Check the UrbanSound_Results.csv for the result comparision for all the methods.

************************************************************************************************************************************************************
up folder contains the saved models and weights.