# Image-to-Image_Translation_GANs

## ** Pix2Pix GAN based Image translation - A Project Report **
## Presented to Prof. Nick Brown

By
1. Aniruddha Tambe (002101113)
2. Kinjal Thakkar (001568960)

## Abstract
To advance the domain knowledge of artificial neural network computing, understanding & implementing Generative Adversarial Networks (GANs) is crucial. This portfolio project involves implementing a Pix2Pix model–a conditional GANs model - by programming the key concepts of encoders, decoders, and generator & discriminator models using Keras. The composite model is then run for predefined calculated training steps. The results of this implementation are saved over 100 epochs as model.h5, after every 10 epochs. This model can be used on unseen Satellite image data to generate faithful translation as Google Map images.

## Execution flow
1. Importing the python libraries
2. Load dataset
a. Call load_images(path,size=(256,512))
Function returns numpy array of decoupled images
3. Display the decoupled images
4. Create the GAN
a. Define the encoder block
Add Conv2D, batch normalization and activation layers
b. Define the decoder block
Add Conv2D, batch normalization, dropout and activation layers
c. Define generator
Add encoder, bottleneck & decoder model
d. Define discriminator
Add multiple conv2D + relu layers , batch normalization layers, sigmoid activation layer
5. Utility functions
a. Define summarize performance
Function summarized performance on each epoch
b. Define generate fake samples
Function returns a batch of fake images
c. Define generate real samples
Function returns a batch of real images
6. Training the model
a. Set the discriminator & generator
b. Set the composite GAN model
c. Call the train model by passing above models
d. Run model for specified epochs – Save each 10th iteration as a model.h5 & output image files

## Conclusion
After using the techniques mentioned in the “Image-to-Image Translation with Conditional Adversarial Network” paper, we can justify the efficacy of the pix2pix model (generator-discriminator) in effectively generating a 256x256 target image of relatively close likeliness.
