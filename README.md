# Topic-Modeling

In this repository, you will find a project I had done during my undergraduate studies on Topic Modeling in Natural Language Processing (a comparative study on various models). Initially, a Spam-Ham classifier and Disaster Tweet classifier were developed using LSTM models with embeddings. Preprocessing methods like cleaning, tokenization, and GloVe embeddings were employed. A Multi-Class Topic Modeling task on news articles using GRU layers demonstrated good accuracy. Later, a combined dataset with four tweet classes was created, and models like LSTM with GloVe, GRU with Universal Sentence Encoder, and BERT with Latent Dirichlet Allocation were tested. Evaluation metrics included accuracy, precision, recall, and F1 scores, achieving decent results across tasks.


| Problem                         | Repository |
| ------------------------------- | - |
| Spam-Ham Message Classifier(Attempt 1) | [CLICK.](https://github.com/Nikitha-Rajendran/spam-ham-message-classifier-1)  |
| Spam-Ham Message Classifier(Attempt 2) | [CLICK.](https://github.com/Nikitha-Rajendran/spam-ham-2) |
| Spam-Ham Message Classifier(Final) | [CLICK.](https://github.com/Nikitha-Rajendran/spam-ham-final)       |
|Disaster Tweet Classifier| [CLICK.](https://github.com/Nikitha-Rajendran/Disaster-Tweet-Classifier)|
| Multi-Class Topic Modeling | [CLICK.](https://github.com/Nikitha-Rajendran/multiclass-modeling)   |

Given below is a tabular summary:

|Task|Dataset Details|Preprocessing|Model and Architecture|Training Results|Test Results|
|-|-|-|-|-|-|
|Spam-Ham Classifier|2550 emails (train), 450 emails (test), 20% validation split|Cleaning, removing stopwords, tokenization|LSTM with embedding layer, binary cross-entropy loss, RMSprop optimizer|Loss: 0.0105, Accuracy: 0.9959, Val Loss: 0.0435, Val Accuracy: 0.9824|Loss: 0.0243, Accuracy: 0.9889|
|Disaster Tweet Classifier|6090 samples (train), 1523 (validation), 3263 (test)|Cleaning (removing URLs, special chars, numbers), stopword removal, lemmatization, tokenization|LSTM with GloVe embedding layer, binary cross-entropy loss, Adam optimizer|Loss: 0.4520, Accuracy: 0.8095, Val Loss: 0.4395, Val Accuracy: 0.8096|Accuracy: 0.77719|
|Multi-Class Topic Modeling|1891 samples (train), 334 (test), 20% validation split|Cleaning, stopword removal, lemmatization, tokenization|GRU, GloVe embedding layer, sparse categorical cross-entropy loss, Adam optimizer|Loss: 0.1092, Accuracy: 0.9712, Val Loss: 0.1359, Val Accuracy: 0.9657|Loss: 0.1179, Accuracy: 0.9641|
