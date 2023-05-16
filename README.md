# CovidPneumoniaDetectionUsingXceptionCNN

The recent COVID-19 global pandemic proved to be a very difficult challenge for many researchers for coming up with effective solution that could break the chain of infection. One of the most efficient solution was through early diagnosis and contact tracing. For faster detection of presence of COVID-19, an optimal machine learning algorithm is needed. This algorithm would analyze X-Ray imaging data and diagnose the patients with high accuracy. Our research project explores the concepts of Deep Learning models namely Convolutional Neural Networks (CNN), DenseNet and Xception that could efficiently classify chest X-Ray images into three labels: COVID-19 infected, Viral Pneumonia infected and Normal condition in human lungs.

A. Collection of Dataset In this study, the dataset has been obtained from an open source Kaggle repository created by a team of researchers from Qatar University, University of Dhaka, Bangladesh and medical professionals from South Asia. The dataset contains chest X-Ray images classified into three labels: COVID-19, Viral Pneumonia and Normal conditions. There are 15153 images available for input which comprises of 3616 images mapped to COVID-19, 10193 images mapped to normal condition and 1345 images mapped to viral pneumonia. The dataset which was updated in February 2022 sizes up to ~900MB in size.

B. Image Preprocessing One of the important phases in the input data preprocessing was to resize the chest X-Ray scan images to a uniform size so that the machine learning models are able to extract maximum information from each image. Depending on the model we wanted to train, the size of the image varied. For Convolutional Neural Network, images were resized to 255 x 255. For both DenseNet and Xception models, image sizes were taken to be 224 x 224. The sizes were the recommended standard values for the mentioned models. The images were also converted from BGR format to RGB as required by Deep Learning models. Finally, the dataset was split in an 80:20 ratio for obtaining the training and testing datasets. The testing dataset for further divided into 50:50 ratio for testing and validation datasets.

![image](https://github.com/khanchandaniashish/CovidPneumoniaDetectionUsingXceptionCNN/assets/113738003/c013d8c5-40a7-41f6-8ac3-85e5ecaa48af)


The Inception model works on the idea that multi-scale convnets have the potential to learn more as they extract features at myriad scales. It also follows the idea that the CNN needs to be large with several layers to be highly performant. A Naive Inception model would consist of an Input layer, followed by 1x1, 3x3, and 5x5 convolutions, a Max pooling layer, and a concatenation layer. This leads to high-performance gains as the ability to extract information increases due to different kernel sizes contributing to better feature extraction. However, these are computationally expensive and are prone to overfitting due to their huge size
To overcome this, Xception builds on the same principles with one major difference: instead of going deeper and adding more layers, go wider. Xception is based on depth wise separable Convolution layers. It can be visualized as a stack of wide convolutions with residual connections. This makes it very simple to define and implement using any Library such as Keras




![image](https://github.com/khanchandaniashish/CovidPneumoniaDetectionUsingXceptionCNN/assets/113738003/d60a7e04-1134-414e-a1ed-931d3df00c22)


OVERALL COMAPRISION OF VARIOS CNN's :

![image](https://github.com/khanchandaniashish/CovidPneumoniaDetectionUsingXceptionCNN/assets/113738003/f9470f9b-2b08-44a2-b6ac-2d9ef7d18ed5)
