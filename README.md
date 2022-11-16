# Melanoma Detection
> Using 9 different sets of lesion images, a multiclass classification model is made. Each set represents a particular type of cancer. In which, we are intrested in detection of melanoma (a type of skin cancer). 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)

## General Information
- First, a baseline model is made with a rescaling layer followed by 3 sets of convolution, batchnormalisation, maxpooling and dropout layers. With each set, the number of kernels in convolution layer is increased i,e 16,32 and 64 kernels in first, second and third set respectiely. Then conclusions were made by dividing train set into training and validation sets.
- Then second model was built. This time with same model configuration (same as baseline model) and an added augmentation layer. This increased the accuracies in conclusion part.
- Finally, Augmentator was called upon. And the augmentator pipeline was initialised. This pipeline created an ouput folder for each of the 9 classes, which contained 500 augmented images for the respective class. Thus, increasing the dataset size by 4500 images and drastically decreasing the class imbalances.
- The augmentator was implenented with only the baseline model and excluding augmentation layer (which was added in second model), thus giving amazing train as well as validation accuracies. 

## Technologies Used
- tensorflow - version 2.10
- CUDA - version 11.2
- cudnn - version 8.1
- python - version 3.9.12

## Contact
Created by [@pavanharde] - feel free to contact me!
