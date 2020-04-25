Context

Flickr674_CIRAF_10 datasets was created for Metropolia University of Applied Sciences Artificial Intelligence and Machine Learning IT00DP82-3002 course work. It was an opportunity to test Deep Learning capabilities for photo classification. The idea is to teach the model using CIRAF-10 and validate the model with photos extracted from Flickr.

Content

Two datasets were utilized. CIRAF-10 is for model teaching, testing and verification and flickr674_CIRAF_10.zip for validation. Flickr674_CIRAF_10.zip contains 674 32*32 pixel photos downloaded from Flickr through Flickr API.

There are ten classification classes: 
0: airplane
1: automobile
2: bird
3: cat
4: deer
5: dog
6: frog
7: horse
8: ship
9: truck

You can make your own Flickr dataset using the following recipe:

1. To get a "key" and "secret", go to https://www.flickr.com/services/api/

2. Download images from Flickr

First run flickr.py using for example: python flickr.py airplane 100

Then run python get_images.py airplane.csv

The codes are from: https://towardsdatascience.com/how-to-use-flickr-api-to-collect-data-for-deep-learning-experiments-209b55a09628


3. the downloaded photos needs to be cropped and rezised to 32*32 pixels. At the same time files names are modified so that the file name starts with number indicating the classes and the "_" for example 0_airplane_1.jpg. The photos are saved as jpegs. You can use photo editing sofware such as Lightroom for the purpose.


4. Jpeg photos needs to changes to png files. Use jpg2png.py fo the purpose.The code is available from https://stackoverflow.com/questions/10759117/converting-jpg-images-to-png

other useful links are:

https://machinelearningmastery.com/how-to-develop-a-cnn-from-scratch-for-cifar-10-photo-classification/

https://github.com/corochann/deep-learning-tutorial-with-chainer/blob/master/src/04_cifar_cnn/cifar10_cifar100_dataset_introduction.ipynb

https://www.kaggle.com/lgmoneda/from-image-files-to-numpy-arrays

https://towardsdatascience.com/3-ways-to-load-csv-files-into-colab-7c14fcbdcb92

http://rodrigob.github.io/are_we_there_yet/build/classification_datasets_results.html#43494641522d3130

https://github.com/subham2203/reimagined-winner/blob/master/cifar_test.py
