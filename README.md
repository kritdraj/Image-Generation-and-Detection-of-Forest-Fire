# Image-Generation-and-Detection-of-Forest-Fire

Every year, wildfires or forest fire, cause immense damage to ecosystems all across the world. The rates of occurrence of this natural disaster is fueled by climate change and is expected to be on the rise in the coming years. Early detection of these wildfires in remote areas is crucial to contain the fire and minimize the damage it causes. Despite the vast research in this area, there are very limited datasets available to train deep networks on, and majority of them are not publicly available. This project aims to generate new images of forest/wildfires using the limited images available on the web by using a Generative Adversarial Network. These images are used to train a classifier to examine its performance with the generated dataset. In addition to this, the classifier is also trained on a images of synthetically produced forest fire from simulated smoke. A comparison of the two methods shows that the classifier trained with the GAN generated images has better generalizability and performs better on real world forest fires images.


Images of forest fires are generated using a Deep Convolution Generative Adversarial Network (DCGAN). The DCGAN is trained with available images of wildfires and images of landscapes. The model generates images with elements of fire and smoke interlaced with the landscapes. These generated images, along with real forest fire images, are used to train a classifier network (VGG16) to classify a presented image as one containing wildfire or not. Another VGG16 model is trained with synthetic smoke dataset as described in the project report and the performance of this model on real forest fire images is compared to that of our model trained with generated images. 

Data collection and preparation was the most labor intensive, time consuming task of this project, reaffirming the 80/20 rule in data science (spending 20% time collecting data, 60%-time cleaning and organizing data, 20% using the data for task at hand). This task provided the invaluable experience of curating data from scratch to make it suitable for training deep neural networks.


![image](https://user-images.githubusercontent.com/57879518/114453202-4dad9f80-9ba7-11eb-82a9-2b0d7cf584e9.png)




