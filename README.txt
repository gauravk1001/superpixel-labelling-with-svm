# SVM-based Classification of Suerpixels of Images into Labelled Groups (MATLAB, Classification of pixels)

This is a experiment to judge the accuracy of parameters of SVM to train a model used to classify parts of images into groups: sky, tree, road, grass, water, building, mountains, and foreground objects  
The tasks done are:
Studied various methods of categorizing parts of an image into meaningful classes  
Used a SVM classifier with varying parameters to extract useful features from a training dataset of about 1K-50K superpixels within images and trained a model using them  
Used the model to predict classes of superpixels occurring in other images and reported the results  


cvip_image_data.mat - Provided data file   

drawregionboundaries.m - used to draw superpixel boundaries on top of an existing image. You should not need to modify this file.

getSPixelFeatures.m  - used to extract features from image data provided. A few features have been defined but you should add additional features to those provided.

makeLMfilters.m - Generates LM filters for texture extraction. You will probably not need to modify this file.

maskimage.m  - used along with drawregionboundaries.m. You should not need to modify this file.

runfile.m  - shows the steps involved icluding functions to call and scripts to run, in order to extract features from superpixels, 

trainSceneLabels.m - uses the in-built Matlab support vector machine to fit a model to the training data (THIS TAKES A VERY LONG TIME TO TRAIN)

testSceneLabels.m  - uses the support vector machine model learned to predict label scores when presented with the test dataset. Optionally, the confusion matrix of the 8 classes is generated and the average accuracy is dispayed as the title of the confusion matrix figure. 



