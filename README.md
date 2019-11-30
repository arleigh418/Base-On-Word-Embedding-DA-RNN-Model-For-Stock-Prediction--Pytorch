# Base-On-Relation-Method-Extract-News-DA-RNN-Model-For-Stock-Prediction


Run model.py.


# Update
### 1.2019/11/30 
1.Us somebody need, I provide three function to show how we count vector, cos and getting sum of each day vector.If cos similar is not achieve your target(e.g. cos>0.7), then we also use top 30% to get more similar article with target center article, like below code:
```
np.percentile({article use} , {per}, interpolation='midpoint')
```
2.Not only add each vector to present one day news vector, we also get average to present one day vector to test(The excel file we provice is avg method). If you are interested, you can try it by yourself.
(I will provide avg method, I can't find where avg method code QQ)


# Reference
1.This porject is referenced this paper:
#### A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction (DARNN)_ Yao Qin, Dongjin Song, Haifeng Chen, Wei Cheng, Guofei Jiang, Garrison W. Cottrell, A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction, IJCAI, 2017.

2.This model modify from here:  https://github.com/Zhenye-Na/DA-RNN

3.We use FASTTEXT to deal with news data ,the method that training fasttext and count relation between news(Cosine) you can reference this   : https://github.com/arleigh418/Word-Embedding-With-Gensim   (Cosine method is in doc2vec_count_cos.py)

--> tips:We add each word's vector from article to present one article vector .

4.We use the 'ta' package to count technical analysis in our data,please reference here: https://github.com/bukosabino/ta

5.Stock price come from : https://finance.yahoo.com/quote/2330.TW?p=2330.TW

# How we do it ? 
Please check Description.pdf.

# Others

1.GOODONE.pkl is the model we train.
2.We know that there are still much left for improvement,we are trying to make this model better. If you have any question , please contact me for free.

