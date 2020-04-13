# National Data Science Challenge 2019

The National Data Science Challenge 2019 topic was "An automatic solution to extract product related information from large volume of images and free text data."

Participants were required to determine the category of the product given its image and title.

Link to Competition: https://www.kaggle.com/c/ndsc-beginner/

## Approach

We used a stacking ensemble method to combine the predictions from 5 Keras sequential models to generate our results.

TfidfVectorizer was used to convert text data into word frequency vectors during data preparation.

We tried using multi-input neural networks with both image and text inputs but led to decrease in our accuracy.

## What could have been done better?

We could have included other models such as BERT and FastText into our ensemble learning.

A learning point from the winning team was to use the [hillclimb ensembling](https://www.kaggle.com/hhstrand/hillclimb-ensembling) algorithm.

## How to run

1. Generate the 5 sequential models by running the [individual-neural-network](individual-neural-network.ipynb) notebook
2. Run the [ensemble-learning](ensemble-learning.ipynb) notebook to stack the 5 models and generate the results
