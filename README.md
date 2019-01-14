# Applying Singular Value Decomposition on Accelerometer Data for 1D Convolutional Neural Network Based Fall Detection
This is a code for the 2019 Electronics Letters paper [Applying Singular Value Decomposition on Accelerometer Data for 1D Convolutional Neural Network Based Fall Detection](https://www.growkudos.com/publications/10.1049%25252Fel.2018.6117/reader) by Heeryon Cho and Sang Min Yoon.

![](https://github.com/heeryoncho/SVD_applied_fall_detection/blob/master/fig/LOSO_Accuracy.png)

## Requirements
This code runs with:
* Ubuntu 16.04
* NVIDIA GeForce GTX 960
* TensorFlow version 1.5.0
* Python 2.7.12

## Downloading Fall Recognition Datasets
Please download the following three Human Activity Recognition benchmark datasets (which include fall activities) from the respective sites and place them inside the 'raw_dataset' folder.
* [SisFall] (http://sistemic.udea.edu.co/en/research/projects/english-falls/)
* [UMAFall] (https://figshare.com/articles/UMA_ADL_FALL_Dataset_zip/4214283)
* [UniMiB] (http://www.sal.disco.unimib.it/technologies/unimib-shar/)

## Remarks
1. Place the unzipped benchmark dataset into the 'raw_dataset' folder. Refer to the directory structure given in the 'raw_dataset' folder's readme.txt.
2. Generate processed (raw or dimension reduced) data by executing codes marked 'gen_XXX.py'. A sample data is given for 'umafall/gen_umafall_dataset_kpca.py'.
3. Build and evaluate 1D CNN models. A sample model is given for 'umafall/umafall_kpca_conv1d_10.py'.

## Citation
If you find this useful, please cite our work as follows:
```
@article{ChoYoon_2019ElectronicsLetters,
  author    = {Heeryon Cho and Sang Min Yoon},
  title     = {Applying Singular Value Decomposition on Accelerometer Data for 
               1D Convolutional Neural Network Based Fall Detection},
  journal   = {Electronics Letters},
  doi       = {10.1049/el.2018.6117},
  year      = {2019},
}
```
