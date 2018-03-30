## Twitter-sentiment

Thie repository contains notebooks for analyzing the sentiment of tweets about self driving cars. The sentiment of each tweet is ranked from 1 (negative) to 5 (positive). 

Here is a sample tweet with sentiment 5: "Autonomous vehicles could reduce traffic fatalities by 90%...I'm in!"

The training data set contains only 5250 tweets, distributed by sentiment (1-5) as: [76, 473, 3287, 1062, 352].


### Getting started

- clone the repo
- create virtual environment
- pip install requirements.txt
- `jupyter notebook` to being the interactive notebook servers

Training and test data are located in the data directory. In the sentAnalysis notebook we try to learn the sentiment solely from the training data. In the sentAnalysisWithPretrainedEmbedding we use a pretrained word embedding based on GloVe.


### Results

We are able to learn to predict the sentiment with a test accuracy of about 64%. This accuracy is not very good, most likely due to the small nature of the training data only 5250 tweets, and each tween only being 140 characters or less. 

### Next steps

To improve the accuracy we would need to gather a larger amount of training data. If it is hard to get enough training data specifically on the subject of self-driving-cars, we may be able to supplement with training data on a related topic, say artificial intelligence, which may use similar words to describe positive or negative sentiments.
