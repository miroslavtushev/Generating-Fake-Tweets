# Generating-Fake-Tweets

Is it possible to generate believable tweets using Machine Learning? How about fake Trump tweets that sound exactly like the original? In this notebook I explore two models to generate fake tweets: **Markov Chains** and **LSTM**. This is a supplemental code for my Medium articles ([1](https://miroslavtushev.medium.com/generating-fake-trump-tweets-using-markov-chains-d75d9a2eed08) and [2](https://miroslavtushev.medium.com/generating-fake-trump-tweets-with-lstm-7c5979229e81)). 

Donald Trump, a former US president, is one of the most controversial presidents in the modern US history. His presidency was remembered by the divisive and sometimes borderline offensive rhetoric. On January 8th, 2021 his Twitter account was suspended due to the attack on the US Capitol.

![download](https://user-images.githubusercontent.com/14366682/143513744-8f6fd2f7-00b7-4700-866f-418463ac0a74.png)
![tweet8](https://user-images.githubusercontent.com/14366682/143513849-a6ef2bba-39b3-47f5-bf7f-a6d69699cc20.png)


In the first part I will demonstrate how to use **Markov Chains** to fake Trump’s tweets. A Markov Chain is a stochastic model describing a sequence of possible events in which the probability of each event depends only on the state attained in the previous event. In the second part I will utilize **LSTM** (Long Short Term Memory): a special case of RNN with the ability to memorize long-term dependencies by preserving the state across cells. By memorizing the context of the tweet, in theory, we should be able to improve upon the traditional context-less models, like Markov Chains.

![LSTM3-chain](https://user-images.githubusercontent.com/14366682/143513775-e259595d-34a1-4187-b792-55523a3e5b01.png)
