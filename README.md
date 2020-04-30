# Toxic_comment_classifiaction
Kaggle competition- https://www.kaggle.com/c/jigsaw-multilingual-toxic-comment-classification?rvi=1

### Downlaod the Dataset from Kaggle
https://www.kaggle.com/c/jigsaw-multilingual-toxic-comment-classification/data

This contains the text of a comment which has been classified as toxic or non-toxic (0...1 in the toxic column). The train set’s comments are entirely in english and come either from Civil Comments or Wikipedia talk page edits. The test data's comment_text columns are composed of multiple non-English languages.

The *-train.csv files and validation.csv file also contain a toxic column that is the target to be trained on.

The jigsaw-toxic-comment-train.csv and jigsaw-unintended-bias-train.csv contain training data (comment_text and toxic) from the two previous Jigsaw competitions, as well as additional columns that you may find useful.

*-seqlen128.csv files contain training, validation, and test data that has been processed for input into BERT.

##### What am I predicting?
Predicting the probability that a comment is toxic. A toxic comment would receive a 1.0. A benign, non-toxic comment would receive a 0.0. In the test set, all comments are classified as either a 1.0 or a 0.0.

##### Files

- jigsaw-toxic-comment-train.csv - data from our first competition. The dataset is made up of English comments from Wikipedia’s talk page edits.
- jigsaw-unintended-bias-train.csv - data from our second competition. This is an expanded version of the Civil Comments dataset with a range of additional labels.
- sample_submission.csv - a sample submission file in the correct format
- test.csv - comments from Wikipedia talk pages in different non-English languages.
- validation.csv - comments from Wikipedia talk pages in different non-English languages.
- jigsaw-toxic-comment-train-processed-seqlen128.csv - training data preprocessed for BERT
- jigsaw-unintended-bias-train-processed-seqlen128.csv - training data preprocessed for BERT
- validation-processed-seqlen128.csv - validation data preprocessed for BERT
- test-processed-seqlen128.csv - test data preprocessed for BERT

##### Columns

- id - identifier within each file.
- comment_text - the text of the comment to be classified.
- lang - the language of the comment.
- toxic - whether or not the comment is classified as toxic. (Does not exist in test.csv.)


##### Output
- Got an Accuarcy ho 88.57%.
![Capture](https://user-images.githubusercontent.com/37845653/80714126-1cf96500-8b12-11ea-9d03-ecf45ca7c539.JPG)


