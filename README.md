# NLP_Clustering

## Clustering for Codekicker.de

Introduction:

In the notebook, have used Nltk as the main library to solve the NLP task of clustering input sentences into 5 groups.

Different text preprocessing techniques such as tokenization, stemming, lemmatization, part-of-speech tagging are done using the nltk library which are specific to German language.

A simple method of clustering sentences based on the frequency counting of the words that matches with the specific tags is performed in this notebook.

Inference:

Using frequency counting with respect to tags is choosen to cluster the input sentences, as it performs better than the other models. It gives better precision and recall scores comparatively.

It is also observed that text pre processing like stemming helped in improving the performance of the model, however using spacy lemmatization did not make any difference with the performance. So i went with stemming. Using pos_tag did not make any difference either.

The precision score of cluster 5 is less, may be because of the insuffiecient tags. However the Recall is good.

Having more tags(words) will help with better clustering. And having more datas could also help with the performance.

Comparing with Other Models:

Have tried different Nlp and Ml models like KMeans Clustering , Agglomerative Clustering, Spectral Clustering, and BERT. But the models did not perform better than this model.

Even after text pre processing, using dimensionality reduction techniques, and normalizing the data, the performance of the model did not improve exponentially. Different hyperparameters were also experimented with each clustering algorithms.

This could be because of not having enough dataset to train the model. By increasing the size of the dataset the model could have better understood the patterns in the data to perform better clustering.

Having an imbalance in the dataset, ie the cluster 4 and 5 have very less data comparatively. Imbalanced dataset could also be a reason to affect the performace in ML models.


Future work:

I could have done data augumentation to increase the number of data to achieve better performance.

I could have also tried different embedding techniques like word2vec, GloVe and FastText.

I could have also used ensemble methods.
