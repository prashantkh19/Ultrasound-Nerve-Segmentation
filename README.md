# Ultrasound-Nerve-Segmentation
Identify nerve structures in ultrasound images of the neck

The task is to segment a collection of nerves called the Brachial Plexus (BP) in ultrasound images. 
A large training set of images is used where the nerve has been manually annotated by humans. 
Annotators were trained by experts and instructed to annotate images where they felt confident about the existence of the BP landmark.

## Dataset
The dataset has been acquired from the Kaggel Competition -[Ultrasound Nerve Segmentation](https://www.kaggle.com/c/ultrasound-nerve-segmentation).

## References
The research paper, [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597) by Olaf Ronneberger,
Philipp Fischer, Thomas Brox is used as a reference. 

## Code
The code is written using [fastai](https://docs.fast.ai/) modules based on [pytorch](https://pytorch.org/docs/stable/index.html).

Kaggle Kernel is used to code the whole project. The notebook can be viewed [here](https://www.kaggle.com/prashantkh19/ultrasound-nerve-segmentation).

#### Environment Details:

`To be updated`

## Configuration 

### Dynamic U-Net
This is the original U-Net architecture.
<p align="center">
<img src="https://user-images.githubusercontent.com/27685757/71420265-4b65c000-269a-11ea-832d-7b5ed7201845.png" />
</p>

The left-part of the architecture is taken pre-trained on [Image-Net](http://image-net.org/) dataset.

#### Reason for the modification:
Taking pre-trained model gives the whole training a head-start in understanding the basic image properties.

##  Results:
- Achieved **top 10%** of the competition's leaderboard on Validation Set with a dice score of around **0.7**.

### Loss Plot

<p align="center">
<img src="https://user-images.githubusercontent.com/27685757/71420709-c29c5380-269c-11ea-9c15-fad5a916605d.png" />
</p>

    The above results are obtained with about half-an-hour training of the chosen architecture. 
