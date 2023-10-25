![image](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/assets/83088512/54beed46-9598-49b7-a6e3-cf724ea89202)# Twitter-Abuse-Detection

This GitHub repository presents a Twitter Abuse Detection Model that aims to identify and combat harmful content on Twitter. The model has been developed and evaluated using two key datasets.

## Dataset Description: 
### Davidson Dataset : 

The ”Hate Speech and Offensive Language Dataset” is a collection of text data curated to study hate speech and offensive language present in online content. The data is compiled using a hate speech lexicon and all the instances are from Twitter. A minimum of 3 coders labeled tweets into classes Hate speech, Offensive and Neither. The final sample consists of 24 000 examples and only about 5% fall into the Hate Speech class. The details of the variables as described by the data collectors are as follows:
* count - Number of users who coded each tweet (min is 3, sometimes more users coded a tweet when judgments were determined to be unreliable by CF).
* hate speech - Number of users who judged the tweet to be hate speech.
* neither - Number of CF users who judged the tweet to be neither offensive nor non-offensive.
* class - Class label for majority of users :
    * 0 - hate speech1
    * offensive language
    * 2 - neither
* tweet - The text message judged by users.

### Founta Et Al Dataset : 

The Founta et al. dataset comprises a diverse collection of annotated tweets, this corpus provides valuable insights into the prevalence and complexities of harmful content online. With meticulous annotations for hate speech, offensive language, and sentiment polarity, the dataset facilitates the development and evaluation of machine-learning models aimed at detecting and
addressing online toxicity. The Founta et al. dataset was the result of a cumulative effort, as mentioned in the paper ”LARGE SCALE CROWDSOURCING AND CHARACTERIZATION OF TWITTER ABUSIVE BEHAVIOR” (Founta et al). The paper describes the data collection process, using crowdsourcing to annotate tweets for hate speech, offensive language, and sentiment. The dataset’s meticulous curation, aided by human annotators, makes it valuable for studying Twitter’s abusive behavior and developing machine-learning models to combat online toxicity. The dataset described  previously consists of 100,000 tweets meticulously annotated through the CrowdFlower platform. Each row of the dataset consists of the tweet followed by the majority label and the number of votes for that majority label. The ”majority label” refers to the most frequently assigned annotation (abusive/hateful/normal/spam) or classification for a particular tweet by human annotators. The ”number of votes for that majority label” indicates how many times the majority label was selected by the human annotators for a given tweet. This information is essential for understanding the level of agreement among annotators regarding content classification.

## Model Description

The study's base model for hate speech detection on Twitter combines traditional classifiers, GloVe embeddings, and transformer-based embeddings. Traditional classifiers like SVM, XGB, and MLP provide a foundation for evaluation. GloVe embeddings capture word meanings, enhancing deep models (CNNs, MLPs, Bi-LSTMs). Transformer-based embeddings, including BERT and ELECTRA, leverage contextual understanding. Text data is represented using TF-IDF for traditional classifiers, GloVe for deep models, and transformer embeddings for advanced models. By exploring various classifier-embedding combinations, the model's versatility and performance are evaluated comprehensively. This adaptive architecture underscores the importance of embeddings and classifiers in effective hate speech detection.

# Output:

### Davidson Dataset
#### SVM
![SVM_Davidson](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/SVM_Davidson.png)
#### XG BOOST
![XG_Davidson](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/XG_Founta.png)
#### MLP
![MLP_Davidson](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/MLP_Davidson.png)
#### BERT
![BertDavidson](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/BertDavidson.png)

### Founta Et Al Dataset
#### SVM
![FountaSVM](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/FountaSVM.png)
#### XG BOOST
![XG_Founta](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/XG_Founta.png)
#### MLP
![MLP_Founta](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/MLP_Founta.png)
#### BERT
![BertFounta](https://github.com/SG-Akshay10/Twitter-Abuse-Detection/raw/main/Output-Image/BertFounta.png)




