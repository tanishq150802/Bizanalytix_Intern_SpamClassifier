# Bizanalytix_Intern_SpamClassifier

Follow **spam_classifier.ipynb** file for all the code.

Install the following requirements while running the notebook on Colab: urlextract

The following results were obtained after training the Artificial Neural Network on the data in easy_ham.tar.bz2 and spam.tar.bz2 files from https://spamassassin.apache.org/old/publiccorpus/ :

1. Training Accuracy : 99.19%
2. Testing Accuracy (70-30 train-test split) : 83.78%
3. Recall : 0.8378
4. Precision : 0.7019

We were asked to convert all the data into a sparse matrix form which prevented us from using the state-of-the-art Scikit-learn classifiers like MLP, Randomforest, Adaboost etc. which take input as a dataframe. As the data was preprocessed into a matrix form, only option was to convert it into a numpy array and train a neural network. Better results are obtained with MLP classifier as suggested in https://github.com/MoazAshraf/Spam-Classifier

PS: I thank Vikram Sir from Bizanalytix for helping me with parsing the emails.
