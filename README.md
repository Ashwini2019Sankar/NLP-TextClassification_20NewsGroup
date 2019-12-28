# TextClassification_20NewsGroupDataset

The 20 Newsgroups data set is a collection of approximately 20,000 newsgroup documents, partitioned (nearly) evenly across 20 different newsgroups. To the best of my knowledge, it was originally collected by Ken Lang, probably for his Newsweeder: Learning to filter netnews paper, though he does not explicitly mention this collection. The 20 newsgroups collection has become a popular data set for experiments in text applications of machine learning techniques, such as text classification and text clustering.

GloVe is an unsupervised learning algorithm for obtaining vector representations for words. Training is performed on aggregated global word-word co-occurrence statistics from a corpus, and the resulting representations showcase interesting linear substructures of the word vector space.

Model summary : I have used the following layers :

Conv1D

MaxPooling1D

Conv1D

MaxPooling1D

Conv1D

GlobalMaxPooling1D

Full Connection

Loss function used is : ‘categorical_crossentropy’ & optimizer used is : ‘rmsprop’ & metrics used
to measure is ‘accuracy’.

Rmsprop : is a very clever way to deal with the problem of vanishing & exploding gradients. It
uses a moving average of squared gradients to normalize the gradient itself. That has an effect
of balancing the step size — decrease the step for large gradient to avoid exploding, and
increase the step for small gradient to avoid vanishing

Model accuracy summary : Initially the test accuracy is better compared to Train accuracy. At
epoch 3, they overlap & after that model tries to overfit & its accuracy is better for training
dataset but less for training dataset.

Model loss summary : In case of loss also similar behaviour is observed. Until epoch 3, the
test loss is less compared to train loss. After epoch 3, the train loss is less compared to test
loss.

The best accuracy achieved for training dataset is : 87.67%
Test dataset accuracy is : 70.87%
