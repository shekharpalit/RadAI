# RadAI

## Data preprocessing


## model creation
Deep Learning FrameWork: Keras
Technique: Transfer Learning -> ResNet 50, Mobile Net, VGG 16

## Approach
In this challenge I used 2 approaches:
Approach 1:
In this approach I used 3 models and train them using real weights and calculate the accuracy of that.
Approach 2:
In this approach I used 3 models, and train them using pre trained weights.

## Model  
### For all the 3 models:
- with / without weights
- Top layer = True (reshape the data)
- Top layer = False
        - manually create a top layer
            - input shape
            - 2 CNN layer
            - Use Activation function(Sigmoid -> because it's a binary classifier)
- Combine top layer with the pre trained model
