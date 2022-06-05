# Text(Docs) Classification

For this bonus excercise I have implemented different models with CountVectorizer and TfidfTransformers simply but it did not return good results to classify the documents. Therefore I have decided to train the model with XgBoost and CatBoost with pretrained Glove Embeddings. After training with both for different size of dimensions of Glove Embeddings, the best model was with 300 dimensions of embeddings applied with CatBoost. I have also applied some tunings. Since there were not all the words of our text in the Glove embeddings I have both applied by just passing those words and randomly generating the embeddings vector for those words and then I have trained the model with both taking the mean and sum of the embeddings vectors. Model with nean of the embeddings was better. I have also fine tunned the scale of normal random number generation. At the end passing the words that are not existed in embeddings were returning better result. Finally I have saved the test predictions to a TSV file to be submitted.**



