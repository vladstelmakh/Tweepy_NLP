Twitter Sentiment Analysis with BERT
This project is focused on analyzing tweets about coronavirus to perform sentiment analysis using the BERT algorithm to predict the sentiment of a tweet (positive, negative, or neutral). In particular, and BERT will be fine-tuned using this dataset to improve the overall performance of the model.
Before feeding the data to the algorithms, the tweets will be carefully cleaned of links, hashtags at the end of sentences, and punctuation marks so that the algorithms can better understand the text and improve their prediction performance.
Such high results can only be achieved by properly cleaning the original data, allowing the algorithms to extract the maximum benefit from it.
In particular, the base model of the Naive Bayes classifier was also trained to perform sentiment classification, resulting in an accuracy and F1 of about 70%.
Training BERT took about 200 minutes per epoch (4 epochs total) on a GPU for each algorithm, since both transformer parameters (over 100 million) were fine-tuned to achieve the best results on a given dataset. It is possible to train only the last transformer layer without fine-tuning the other parameters: however, this usually leads to worse results compared to the fine-tuning approach.
Libraries
Numpy
Pandas
Tensorflow
Matplotlib
Seaborn
re
string
emoji
nltk
sklearn
Imblearn
