# Contains my Machine Learning Journey from the Start

Hi!!!
I have categorized all my notebooks on Image Processing, Natural Language Processing and everything else into different folders all in one place and not lying all over on Github.

## [Image Processing and Research](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/1.%20Image%20Processing%20Basics%20and%20Research)

* **[1. Starting_out](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Image%20Processing%20Basics/1.%20Starting_out.ipynb)**: The very basics of image processing like colour channels, separating them, frequency histograms, and stuff like that while I was starting out

* **[2. U-Net.ipynb](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Image%20Processing%20Basics/2.%20U_Net.ipynb)**:
The U-net on the DRIVE Dataset and the results are saved in the above folder.

* **[3. Dendritic Spine Segmentation](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Image%20Processing%20Basics/3.%20Dendritic_spine_segmentation(U_Net).ipynb)**: Transfer Learning was applied to images of dendritic spines. The same DRIVE Dataset was modified a bit(the images were negated to suit the needs of another dataset where the objects were of high intensity and background was of low intensity) and trained on the same UNet to segment out the dendritic spines from the different dataset.

* **[4. Dendritic Spine Segmentation](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Image%20Processing%20Basics/4.%20Dendritic_Spine_Segmentation(Attention%20U_Net).ipynb)** : The same as the above notebook but with the attention model (reference: Python for Microscripts repo). A concensus based algorithm was used for binarisation of the input images in dendritic spines and the model was trained on the image pair generated with it.

* **[5. Disease Prediction from Medical Imaging( non-intrusive tests )](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/1.%20Image%20Processing%20Basics%20and%20Research/5.%20Disease_prediction_from_medical_imaging(non_intrusive_tests).ipynb)** : A part of research at University of Hyderabad, where I had tried to make a tool which would take in various images like a person's face and drawings and predict what diseases they might possibly have. The models used are really simple. This project however is no longer being actively worked on. Thorough literature reviews and datasets used are included in **[Additional Material](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/1.%20Image%20Processing%20Basics%20and%20Research/Additional%20Material%20(%20with%20the%205th%20notebook%20))**


## [Retinal Image Segmentation](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/2.%20Retinal%20Image%20Segmentation(Research))

* [**SAU-Net.ipynb**](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Retinal%20Image%20Segmentation/1.SA_UNet.ipynb): This contains an implementation of the [**Spatial Attention U-Net paper**](https://arxiv.org/ftp/arxiv/papers/2004/2004.03696.pdf). The model has been tried on the DRIVE Dataset with upto 92% accuracy. This is basically an attention based Convolutional Neural Network model. It is a derivative of the conventional U-net model already in use. Various data augmentation strategies have been used. The images of the test set formed therof are also present in the respective folders. **Areas of improvement**: data augmentation strategies, use of dropblock to be done properly.

* [**Nearest_Neighbour_Algorithms_on_pixelwise_classification_of_DRIVE.ipynb**](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/Retinal%20Image%20Segmentation(Research)/2.KNN_on_pixelwise_classification_on_DRIVE.ipynb): KNN is performed on pixelwise classification of Retinal images on a modified version of the DRIVE Dataset. The modifications to the dataset are the crux of the project, and to be disclosed at a later date in the future. Random undersampling, random oversampling is done to fix the ratio of non blood vessel pixels and blood vessel pixels which are originally in the ratio of 1:10. SMOTE algorithm followed by random undersampling of the over-used classes is done, bringing the ratio of blood vessel pixels to non-blood vessel pixels to 1:5.

## [Neural Networks](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/3.%20Neural%20Networks)

File contains a neural network made from scratch. The intuition, theory and a little maths is included in a blogpost as a sort of tutorial on my blogsite. At first the structure of simple single- layer perceptron is coded and then generalised for n- neurons and layers. It has a very good accuracy of 95.55% on the iris dataset


## [Sentiment Analysis](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/4.%20Sentiment%20Analysis)

Ideas collected from some blogs, sites and other cool resources available on the internet that got me started in sentiment analysis as well as
some of the results I found while playing around with these NLP tools. **The inspiration for each of those notebooks are mentioned as source
in the notebooks.** Trying to recreate these notebooks would be helpful for anyone interested. Constructive criticism is also welcome.

### Description:
Tried to apply my knowledge on the IMDB review dataset for sentiment analysis

### Files:

File-1: How even different vectorisers affect the accuracy of data

File-2: How the different models in Scikit-learn affect the accuracy of predictions

File-3: How ensemble models increase accuracy

File-4: Current methods like LSTM and deep learning(how they affect accuracy)

The Dataset used is here
https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

To upload the dataset on google colab:

https://towardsdatascience.com/3-ways-to-load-csv-files-into-colab-7c14fcbdcb92

Change the runtime to GPU in colab for better performance.

### Youtube Resources for nlp:
NPTEL(Applied NLP): https://www.youtube.com/playlist?list=PLH-xYrxjfO2WyR3pOAB006CYMhNt4wTqp

NPTEL(Some theory is good too. :)): https://www.youtube.com/playlist?list=PLJJzI13YAXCHxbVgiFaSI88hj-mRSoMtI

Krish Naik: https://www.youtube.com/playlist?list=PLZoTAELRMXVMdJ5sqbCK2LiM0HhQVWNzm

## [Created Datasets](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/5.%20Created%20Datasets)
* Blackadder full episodes: Extracted the scripts of blackadder from the web in order to create a dataset for **Natural Language Generation**. This dataset is available on [kaggle](https://www.kaggle.com/soumee2000/blackadderfullscriptsrowan-atkinson) and the [tutorial](https://soumee2000.github.io/technical/Web-scrapping/) is up here on my blog-site.

## [Natural Language Generation](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/6.%20Natural%20Language%20Generation)
**Description**: Deals with a variety of basic techniques That can be used for predicting the next word in a sentence.

* **[Word_prediction.ipynb](https://github.com/SOUMEE2000/Machine-Learning-Stash/blob/main/6.%20Natural%20Language%20Generation/Word_prediction.ipynb)**: deals with preprocessing text, using bigrams, trigrams and LSTMs

## [Digit Classifiers](https://github.com/SOUMEE2000/Machine-Learning-Stash/tree/main/7.%20Digit%20Classifiers):
* Created digit classifiers with the help of simple Neural Networks, Convolutional Networks and GANs.
