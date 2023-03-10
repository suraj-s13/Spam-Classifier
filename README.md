<h1 align="center">
  <br>
  SpamClassifier
  <br>
</h1>
<h3 align="center">In this project I build a model for classifying the Email into spam or ham through the text of the Email using  Logistic Regression.</h3>

## What It Does: 
<p align="center">
  <br>
  <img src="https://miro.medium.com/max/1200/1*_igArwmR7Pj_Mu_KUGD1SQ.png">
</p>

## How It Does:
Extract the text and the target class from the dataset. Extract the features of the test using TF-IDF vectorizer for the Input features.Split the skewed data into shuffled sets using stratified shuffle split in sklearn library. Use standard classifiers to classify the data into spam or ham.
<p align="center">
  <br>
  <img src="https://github.com/ShubhamPy/Spam-Classifier/blob/master/Screenshots/modelLearning.png">
</p>

## Prerequisites:
I would highly recommend that before the hack night you have some kind of toolchain and development environment already installed and ready. If you have no idea where to start with this, try a combination like:
-  `Python`
-  `scikit-learn` / `sklearn`
-  `Pandas`
-  `NumPy`
-  An environment to work in - something like `Jupyter` or `colab`
For Linux people, your package manager should be able to handle all of this. If it somehow can't, see if you can at least install Python and pip and then use pip to install the above packages.

## Dataset:
The Email Spam Collection is a set of SMS tagged messages that have been collected for Email Spam research. It contains one set of SMS messages in English of 5,572 messages, tagged according being ham (legitimate) or spam.

> You can collect raw dataset from [here](mail_data.csv).

The files contain one message per line. Each line is composed by two columns:
- `Category`- contains the label (ham or spam) 
- `Message` - contains the raw text.

## ModelPipeline:
<p align="center">
  <br>
  <img src="https://github.com/ShubhamPy/Spam-Classifier/blob/master/Screenshots/modelLayout.jpg">
</p>

## Components:
-  Using TF-IDF for feature extraction of the text data for the messages.
-  Use splits for skewed data(Since the number of ham are far more than the number of spam messages,the data is skewed)
-  Use stratified shuffled split for the split of skewed data.
-  Use different standard classifiers for classification of the SMS.
-  Compare the accuracy of various classifiers using standard classification metrics

## AccuracyResult:
<p align="center">
  <br>
  <img src="Screenshot 2023-02-11 145755.png">
</p>

## Future Scope:
- Adding this feature in a dynamic website which supports contact-us typo feature.
- Show live user inputs for Ham and Spam  .
