# SOC_2022
Deoldify Videos

L*a*b vs r*g*b

Normally images are stored in rgb format. Which contains amount of red, green and blue at each pixel in range of 0 to 255. Now if we used this model for training  our model it has to predict 3 numbers from a single number with 256*256*256 unique possible set. It would be quite difficute.

![rgb](https://user-images.githubusercontent.com/81369524/181990120-c6d4eb44-f959-4c84-bbc9-db1819142301.jpg)


Fortunately there exists a another formate for storing an image ie Lab. In which L represents brightness of an image, a contains how red-green each pixel is where as b stores how much blue-yellow each pixel is. If we used this formate we will have to find just a and b from given L. Making our work less by one power ie now we have 256* 256 possibilities.

![lab](https://user-images.githubusercontent.com/81369524/181990271-60d3b52d-79d1-4e8b-9dd4-b0fc7b0e640e.jpg)

Guiding paper:

[[1611.07004] Image-to-Image Translation with Conditional Adversarial Networks
](https://arxiv.org/abs/1611.07004)

Gyan of GAN:

GAN is the algorithum behind the trending reel of these people do not exist, motion in a photograph, age changer apps, text to image converter aka NLP (TReCS and XMC-GAN) and as you might have guessed old image colorization. 

Basic idea

It contains 2 ML models, one Generator (G) and other Discriminator (D). G generates fake images. D determines if image is fake. D is a simple CNN model for image classification. It is trained to know what are fake and real images. Then training process of G begins. G is created with U-Net architecture, which is a fully connected CNN, which instead of pooling upsamples increasing the resolution in the output. we initiate G with random noise, then generate images.





Resources:

for more about U-net: https://lmb.informatik.uni-freiburg.de/people/ronneber/u-net/

https://towardsdatascience.com/reshaping-numpy-arrays-in-python-a-step-by-step-pictorial-tutorial-aed5f471cf0b

https://machinelearningmastery.com/how-to-load-and-manipulate-images-for-deep-learning-in-python-with-pil-pillow/

https://www.google.com/amp/s/www.geeksforgeeks.org/how-to-convert-images-to-numpy-array/amp/

Basic image processing (three parts)

https://www.kdnuggets.com/2018/07/basic-image-data-analysis-numpy-opencv-p1.html

https://www.kdnuggets.com/2018/07/image-data-analysis-numpy-opencv-p2.html

https://www.kdnuggets.com/2018/09/image-data-analysis-python-p3.html
