# RadAI

## Data preprocessing
- The data set is not uploaded, because of its heavy size.
load and resize the images using the helper function get_data(), and store them in 2 variables (x, y) as images and lables



## model creation
- Deep Learning FrameWork: Keras
- Technique: Unet 
## Approach
In this challenge I used a famous CNN network architecture called Unet which was developed for biomedical image segmentation

-It consists of the repeated application of two 3×3 convolutions, each followed by a batchnormalization layer and a rectified linear unit (ReLU) activation and dropout and a 2×2 max pooling operation with stride 2 for downsampling

-The purpose of this contracting path is to capture the context of the input image in order to be able to do segmentation.

-Every step in the expansive path consists of an upsampling of the feature map followed by a 2×2 convolution (“up-convolution”) that halves the number of feature channels, a concatenation with the correspondingly feature map from the contracting path, and two 3×3 convolutions, each followed by batchnorm, dropout and a ReLU.

-The purpose of this expanding path is to enable precise localization combined with contextual information from the contracting path.

-final layer a 1×1 convolution is used to map each 16- component feature vector to the desired number of classes.

##Note
-This model is developed and tested in a underpowered laptop(macbook air), so the dataset used in this is 1/3 of the orignal dataset. However, the model will work perfectly in a large dataset.
-This model is designed to run on a GPU (cuda not used, but we can use it in future work)

