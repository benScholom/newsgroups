# newsgroups

A classification of newsgroups from the newsgroups dataset available on scikit learn.

Getting Started:

1. Ensure all the appropriate python packages are installed (pip install [package_name])
	a. numpy
	b. pandas
	c. scikit-learn
	d. matplotlib
	e. nltk
	f. jupyter
	g. hyperopt (may require downgrading networkx to version 1.11 to work if you already have a later version)

2. In the command line, go to the directory where the notebook is stored and type "jupyter notebook"

The notebook:

The notebook implements both a k-means clustering algorithm and classification algorithm (Stochastic Gradient Desent Classifier) on the newsgroups data. 
It is an initial draft based on 1-2 days of work and it includes preprocessing such as word stemming and removal of stop words and irrelevant characters, dimensionality reduction to assit the clustering,
 and hyperparameter optimization to improve the algorithm. Key decisions and the reasoning behind him are elaborated upon in the notebook itself.

Going forward:
 

1. Preprocessing - I used word stemming because it was simple and quick to implement. With more time, I would like to implement lemmazation instead
	which is more accurate though more time consuming. Additionally, I would like to spend more time cleaning out words that may be unnecesary.
	I feel that better data is more important than a better algorithm, and more time should be spent ensuring the data is as clean and relevant as possible.

2. Dimensionality reduction - I was able to roughly figure out the optimal number of dimensions to improve the clustering algorithm. However, the algorithm is still not as robust
	as I would like. In the future, I may try non-linear dimensionality reduction techniques to see if they lead to better results.

3. Classification - The SGDClassifier has solid performance, but I would like to try to implement deep learning with word2vec, which would take more computing power and time to implement
	but may yield better results. Additionally, I would like to spend more time on hyperparameter optimization, as I feel that the current implementation could be improved. Also, preprocessing
	algorithms like TFIFD could also be optimized.