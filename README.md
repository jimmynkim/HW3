# Reproducibility Project
## [Re] DeepGlobe 2018: A Challenge to Parse the Earth through Satellite Images

### Reproducibility Summary

*Methodology*
Optimization:
RMSprop optimization is popular optimizer choice for segmentation tasks but adamW could also handled by a UNet model.
Learning rate:
selecting a too large learning rate isn't necessary.
L2 regularization: 
we're not utilizing L2 regularization.

*Results*

*What was easy*
The paper is made up of clear and concise codes and is informative.

*What was difficult*
Finding the appropriate learning rate, batch size, and other hyperparameters was difficult. This will need to be adjusted through experimentation, and it may take time to determine which value is optimal. Code execution takes too long. Running a model takes approximately 10 hours or more, so if an error occurs, it must be executed again from the beginning, which is time consuming.

### 1. Introduction
Automatic classification and segmentation of land cover is critical for sustainable development, autonomous agriculture, and urban planning. DeepGlobe 2018: A Challenge to Parse the Earth through Satellite Images paper introduces the challenge of automatically classifying land cover types, This problem is defined as a multi-class segmentation task that detects urban, agricultural, grazing land, forests, water, barren land, and unknown areas. Here, we intend to classify using UNet additionally using the U-Net: Convolutional Networks for Biomedical Image Segmentation paper.

### 2. Scope of reproducibility

### 3. Methodology
Optimization:
RMSprop optimization is popular optimizer choice for segmentation tasks but adamW could also handled by a UNet model. Its adaptive learning rate mechanism can help navigate complex loss landscapes, potentially leading to faster convergence and improved segmentation accuracy. 

Learning rate:
RMSprop adjusts the learning rate itself, so selecting a too large learning rate isn't necessary.

L2 regularization: 
While weight decay acts as L2 regularization and can prevent overfitting in the model, in this case, with these hyperparameters, we haven't encountered overfitting, so we're not utilizing L2 regularization.

### 4. Results
Photos of results when you run Unet 

![image](https://github.com/jimmynkim/HW3/assets/75557016/8ef302a0-3e4f-43f6-a516-5c721f3c9ea7)
IoU 값은 0.4213

### 5. Discussion


### 6. Conclusion
RMSprop  optimization is popular optimizer choice for segmentation tasks  like those handled by a UNet model. Its adaptive learning rate mechanism can help navigate complex loss landscapes, potentially leading to faster convergence and improved segmentation accuracy. 
