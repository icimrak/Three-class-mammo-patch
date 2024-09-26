# Three-class-mammo-patch
ResNet model classifying patches into three classes: 1. containing cluster of malignant microcalcifications, 2. containing cluster of benign microcalcifications, 3. background (can be normal tissue, macrocalcifications, massses)) 

Convolutional network model trained for classification of patches into three categories: 
1. containing cluster of malignant microcalcifications,
2. containing cluster of benign microcalcifications,
3. background (can be normal tissue, macrocalcifications, massses))

The files must be concatenated by e.g. the macos/linux command

cat model* > PRETRAINED_RESNET101_ADAM_LR5e-06_BS8.tar

Original model file was split using the command
split -b 22000k PRETRAINED_RESNET101_ADAM_LR5e-06_BS8.tar model

After the files modelaa .. modelah are merged into one file PRETRAINED_RESNET101_ADAM_LR5e-06_BS8.tar, the provided script example1.py demonstrates a classification of two patches.

This is a Suppementary material of a paper:
Enhancing Breast Microcalcification Classification: From Binary to Three-Class Classifier
https://ieeexplore.ieee.org/abstract/document/10516355

When using this model, please cite the following:
A. Mračko, I. Cimrák and L. Vanovcanová, "Enhancing Breast Microcalcification Classification: From Binary to Three-Class Classifier," 2024 35th Conference of Open Innovations Association (FRUCT), Tampere, Finland, 2024, pp. 473-481, doi: 10.23919/FRUCT61870.2024.10516355.
