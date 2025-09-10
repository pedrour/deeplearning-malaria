MIT Applied Data Science program

Malaria Detection using Deep Learning

Background

Malaria is a serious disease that infected 229 MM people and caused 409K deaths WW in 2019. Annual spent for testing and treatment amounted $3B USD in 2019
Most common testing techniques require manual result interpretation, with a average hourly cost of $6.8/h or an estimated ~$778 MM USD annually. ML technology can help automate part of this manual intensive process and help reduce detection costs.

I develop a proof of concept Deep Learning system using novel techniques like Convolutional Neural Networks that can predict with 96% accuracy if a given red blood sample is infected or not. 
Based in my initial experiment results, we present our learnings and recommended next steps to build a productionized system to help automate Malaria detection.


Overview

* I implemented Tensorflow/Keras CNN models following the VGG16 (Very Deep Convolutional Networks for Large-Scale Image Recognition) architecture, a widely adopted model for image classification.
* I trained our system with ~25K uninfected/infected images, and validate it with a sample of 1.3K images. 
* I used techniques of image preparation and preprocessing to increase accuracy (resizing, normalization, augmentation).
* I used transfer learning, meaning we used pre-trained parameters on other image data sets.
* I evaluated 4 different models, where we tried different CNN techniques and architectures (for example, hyperparameter tuning and data augmentation)


Experiment results

* My best performing model achieved a 96% accuracy and precision detecting if a given sample is infected or not. The model with highest accuracy was our third model, which consisted on original data set + VGG-16 (without augmentation)
* I evaluated the performance of our model using training vs. validation accuracy and precision analysis, and performed predictions on test data. 

Recommended Next steps:

* Further research CNN models, including expanding the data set available, and using other techniques like different pre-trained CNN models, hyperparameter tuning; to improve model accuracy and reduce the risk of misdiagnosis.
* Design a ML E2E system architecture for productionizing the system (including data acquisition and processing, model training, execution and deployment) 
* Define data security and privacy mechanisms that are compliant with regulations and that properly handle patient/sample data following best practices.
* Address potential ML ethics concerns in addition to privacy, such as selection bias, discrimination on how to use the results, and the role of human judgement (or the lack of).
* Define a viable business plan that defines how the system will be integrated on actual medical processes, costs and a roll out strategy.
