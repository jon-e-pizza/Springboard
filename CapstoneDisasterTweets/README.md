# Diagnosing a Disaster Tweet

In this project we detail the creation of a model with the intent to successfully predict whether a tweet is talking about an ongoing disaster. We apply text preprocessing methods to create a reduced TF-IDF representation of the labeled tweets provided at https://www.kaggle.com/c/nlp-getting-started/overview. We then use these transformed tweets to fit machine learning classifiers Random Forest, XGBoost, and Naive Bayes. We also train neural networks to classify the same. 

Within this directory are the files:
- **[Final Report](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/Recognizing-Disaster-Tweets_Capstone-2-Final-Report.pdf)** detailing our full process from initial proposal to model production, to next recommendations
- **[Milestone 2 Report](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/Recognizing-Disaster-Tweets-Capstone-2_Milestone-Report-2.pdf)** detailing our initial proposal for this investigation to each step in the process of producing models
- **[Milestone Report](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/Recognizing-Disaster-Tweets_Capstone-2-Milestone-Report-1.pdf)** an early revision detailing our initial proposal and exploration of our problem space
- **[Presentation](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/Diagnosing-the-Disaster-Tweets-slides.pdf)** a slide presentation to review the most essential details of the project

And directories:
* **[data_wrangling](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneDisasterTweets/data_wrangling)** containing our text preprocessing steps
    * **[Python Notebook](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/data_wrangling/preprocessing.ipynb)** Detailing steps and code in processing our text and producing TF-IDF and lda representations

* **[data](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneDisasterTweets/data)** containing our input data set from kaggle, as well as the output of our text preprocessing steps, binary except for:
    * **[Input Data](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/data/kaggle_training.csv)** Labeled tweets provided by kaggle
    * **[Processed Data](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/data/processed_kaggle_training.csv)** Processed tweets from kaggle after removing stops words and lematicizing

* **[data_exploration](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneDisasterTweets/data_exploration)** containing our summarization of the problem space
    * **[Python Notebook](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/data_exploration/eda.ipynb)** Detailing steps and code analysing the differences between our two classes of tweets

* **[machine_learning](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneDisasterTweets/machine_learning)** containing machine learning modeling processes used in analysis
    * **[Python Notebook for Traditional Classifiers](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/machine_learning/trees_and_bayes.ipynb)** Detailing code for machine learning models and steps taken to arrive at optimal models
    * **[Python Notebook for Neural Network Classifier](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/machine_learning/NeuralNetworks.ipynb)** Detailing code for creating word vectors and then classifying tweets with an LSTM layer that takes them as input
    * **[word vectors](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneDisasterTweets/machine_learning/word_vectors.csv)** The file containing the vectors produced in the first part of our machine learning