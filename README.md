# Toxic-Comment-Classification
This was my submission to the kaggle competition: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge.  This was a challenge to develop a model to automatically find and moderate toxic comments on Wikipedia.

## Strategy
1. I first used a basic Logistic Regression model to make predictions.  Logistic Regression is extremely fast and useful for binary classifications, so it was a great starting point.
2. I then trained a neural network to pick up on less noticeable trends in the data.
3. Adding pretrained word embeddings (Facebook's FastText) improved the accuracy of my predictions by quite a bit.
4. I was then curious to see how my model would do on outside data, and used Twitter API to scrape tweets about Uber.  I ran those tweets through my neural network to see what kind of toxic comments were beind made about the company.
