# Urdu_Caption_Generation-G1K
“This repository contains code and results for the Course Project by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This repository is only for learning purposes and is not intended to be used for commercial purposes.”

Course Link: http://im.itu.edu.pk/deep-learning-spring-2020/

# Abstract:
Image caption generation has been seen as a quite difficult task mainly due to two reasons the first being the ability to solve computer vision challenges of detecting and determining objects in a given image and also to capture and express the relationships of these objects in a natural language. Moreover, due to the sparsity of annotated resources in languages other than English, this task becomes more challenging and arduous. Also, a lot of work has already been done in this regard for English language as compared to other languages like urdu which adds to the complexity of this task. Our work basically focuses on generating high quality Urdu captions from images by capturing image features through CNN, then generating text features through word embeddings. Finally generating captions through greedy search. For generating captions in Urdu we manually prepared a translated subset of Flickr8K dataset to cater the complexity of the problem to some extent. Our selected subset mainly focuses on images containing boys doing various activities. Urdu is a diverse language in comparison to English and its grammar makes it quite difficult to work with. However, we employed an urdu word2vec model to cater this issue. 

# Dataset:
* We have used a subset of Flickr8K dataset containing images of boys involved in various activities.
* Total 550 images with 2750 captions (5 captions per image) are present in the dataset
* We have manually translated these captions from english to Urdu.
* Dataset link: https://drive.google.com/drive/u/1/folders/1mIZghxXLIYE4lRN3pOUyvZrwcMqYM_rZ

![dataset](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/images/dataset.PNG)

# Model Architecture:

We focused to build on the work of Vinyal et. al. [2]. InceptionV3 was employed as CNN to extract the features of the image. We have generated urdu word embeddings using urdu word2vec model by urduhack to genearate urdu captions for images. We have employed the GreedySearch approach and used LSTM language model for caption generation.  

![Flow diagram](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/images/model.png)

# Pyhton Notebooks:

[1. Extracting feature Vectors from Images](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/notebooks/1.Extracting%20feature%20Vectors%20from%20Images.ipynb)
[2. Extracting Text Features](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/notebooks/2.%20Extracting%20Text%20Features.ipynb)
[3. Training Captioning Model](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/notebooks/3.%20Training%20Captioning%20Model.ipynb)
[4. Caption Generator](https://github.com/msds19012/Urdu_Caption_Generation-G1K/blob/master/notebooks/4.%20Caption%20Generator%20.ipynb)

# Results:

