# Project Overview
###### <i>UC Berkeley MIDS `Applied Machine Learning` Group Project</i>

### Objective: 
The goal of this project is to classisfy breast cancer mount slide images into cancerous vs. non-cancerous. The images were obtained from the Kaggle website. We trained a baseline model and then three additional models with include Random Forest, CNN (Convolutional Neural Network), and CNN with transfer learning.

### Scoring Criteria:
The AES system evaluates essays across six key analytical dimensions: cohesion, syntax, vocabulary, phraseology, grammar, and conventions. Each dimension reflects a specific aspect of writing proficiency, with scores ranging from 1.0 to 5.0, in increments of 0.5, where higher scores represent greater proficiency.

### Technical Approach:
We employed both **BERT (Bidirectional Encoder Representations from Transformers)**, trained on formal text, and **BERTweet**, trained on informal language such as tweets, to assess student essays. These models capture both semantic nuances and structural elements, mapping linguistic features to scores in an ordinal framework. To enhance scoring precision, we used **Mean Columnwise Root Mean Square Error (MCRMSE)** regression loss, ensuring a more accurate and consistent scoring range.

### Performance Enhancement Techniques and Performance Results:
Starting with a frozen BERT-base-cased model as a baseline, we experimented with unfreezing various numbers of lower layers and adjusting hyperparameters on both BERT and BERTweet to allow the models to learn from different usages of English during training. We also applied clustering and stratified k-fold cross-validation to check for patterns in score distributions and to ensure our model generalized well across different data partitions, particularly at the lower and higher ends of the scoring scale.

However, since the analytical measures followed a normal distribution, applying K-means clustering and k-fold cross-validation did not significantly enhance model performance. Our best result was a moderate MCRMSE loss score of 46%, achieved with 12 trainable layers in the BERT transformer model.

Please refer to the link below for more details on the teamwork:
* [Team GitHub](https://github.com/TatiannaD/w207_fall2022_mlproject//)
