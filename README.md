# Sentiment Analysis With Pytorch and tried WandB

In this series we'll be building a machine learning model to detect sentiment (i.e. detect if a sentence is positive or negative) using PyTorch and TorchText. This will be done on movie reviews, using the IMDb dataset.

# INTRODUCTION 
Here, I'm using Recurrent neural network :
Recurrent neural network is like not doing anything from scratch, same with our understanding of each word based on the previous words.
We have some memory saved and if some words related to the memory comes up then we use the saved memory to understand the words (memory can be called as Vocubalary).

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fcolah.github.io%2Fposts%2F2015-08-Understanding-LSTMs%2F&psig=AOvVaw2riCsmLKdrahaUIwf-jvbJ&ust=1596636221096000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNDYzM7bgesCFQAAAAAdAAAAABAD">

# PREPARING THE DATA
Here I'm using TorchText, TorchText is a library that makes :
Read the data, 
Tokenize the text, 
Create a mapping from word to a unique integer,
Convert the text into lists of integers.

One of the main concepts of TorchText is the Field. These define how your data should be processed. In our sentiment classification task the data consists of both the raw string of the review and the sentiment, either "pos" or "neg".
The parameters of a Field specify how the data should be processed.

The IMDb dataset consists of 50,000 movie reviews, each marked as being a positive or negative review.

loss function

The loss function here is binary cross entropy, 
The BCEWithLogitsLoss criterion carries out both the sigmoid and the binary cross entropy steps.

<img src = "charts/Section-1-Panel-0-tjtppywk.png width = 100 height = 50">
<img src = "charts/Section-1-Panel-1-gjwyiwdgb.png width = 100 height = 50">
<img src = "charts/Section-1-Panel-2-qldtutsu.png width = 100 height = 50">
<img src = "charts/Section-1-Panel-3-lclwzpwtu.png width = 100 height = 50">
<img src = "charts/Section-1-Panel-4-ncf22sl6r.png width = 100 height = 50">

Tried Wandb for graphs, these are some images of the accuracy and loss for the range of epochs.
https://app.wandb.ai/pratikraut_/text_classification_project?workspace=user-pratikraut_
You can visit this links.
