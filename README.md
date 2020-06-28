# Detecting Sarcasm in Reddit Comments

This was a small project I worked on, with Rubini and Vikram, during my 2020 Summer Internship at Carnegie Mellon University.

## Aim

The aim is to detect sarcasm in comments found on Reddit, using the [Sarcasm on Reddit](https://www.kaggle.com/danofer/sarcasm) dataset available from Kaggle. Through this, we also aim to identify features that are indicative of sarcasm, and explain our models' predictions.

## Methodology and Results

We experimented with TF-IDF and BERT Sentence Embeddings to extract features from text. We tried using various combinations of features, such as using only the comment, its characteristics and also its parent comment, to provide context. Additionally, we tried to use PCA for dimensionality reduction.

The classifiers we used include the Random Forest Classifier, Gradient Boosting Classifier and the Multi-Layer Perceptron, among others.

Our best-performing model was a Random Forest Classifier trained on TF-IDF features extracted from raw text (comment and parent) and also the comment's characteristics such as the subreddit and author. It obtained an F1-Score of 0.66 on the validation set. The comment's characteristics were deemed as very important features by the models we built.

## Code

The code is available as three Jupyter Notebook files, simply start up a Jupyter Notebook server and run the code. Ensure that the dependencies are installed before you run the code. To do so, simply execute this command in the Terminal:

```bash
pip install -r requirements.txt
```

## Presentation

Our [presentation](Sarcasm.pdf) is also available in this repository, and provides more information.
