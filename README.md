# Project-3-reddit-classification
# Project-3-reddit-classification
------------------------------------------------------------------------
## Contents:

  - Problem Statement
  - Executive Summary
  - Data Dictionary
  - Conclusions and Recommendations
------------------------------------------------------------------------

## Problem Statement

Since video streaming service like Netflix, Disney plus and HBO become more and more popular, many people spend more times on television show and movie, while some of them prefer television show over movie becuase tv shows has more complex story, more character and more time to digest. Some people prefer movie over tv show because it take less time and it has more special effect. As a part of data science team at film and television production company, I was tasked with creating a model that will be able to take a reddit post and classify which posts were talking about movies and which posts were talking about TV to see current trends for. Allow the company to make movies or Television programs according to consumer demand

------------------------------------------------------------------------

## Executive Summary

To classify which post is about movie or television, I used data from sub reddit movie suggestions and television suggestions. This project aims to created a model that can correctly classify the post by using model like logistic regression, multinomial naive bayes and support vector machine, also create confusion matrix to find accuracy rate, misclassification rate, true positive and true negative rate.

------------------------------------------------------------------------

## Data Dictionary

| Column          | Type         | Description                                |
| :---------------: | :----------: | -----------------------------------------: |
|subreddit       | str       | Overall material and finish quality        |
|title       | str          | title of the post |
|selftext     | str        | text of the post  |
|text        | str        | combined of topic and text of the post             |
|y   | int       | label of the target to use in classifiation 0 is tv suggestions and 1 is movie suggestions  |

------------------------------------------------------------------------

## Conclusions and Recommendations

**Conclusion**

Based on the train and test accuracy, it appears that multinomial naive bayes performed the best out of three. With train accuracy rate at 94% and test accuracy rate at 85%, multinomial naive bayes also has less overfit when compared to logistic regression and support vector machine. On unseen data this model correctly predicted that 189 posts are movie suggestion and 209 posts are television suggestion. The top 10 words that use to classificaty for movie and television are overlapping such as 'like', 'watch','look','good' and 'realli'.
        

**Recommendation**

- This project use only 3 models (Logistic regression, Multinomial naive bayes and Support vector machine) maybe try another classification model.

- Try another feature extraction like Tfidf vectorizer or hashing vectorizer

- Try remove some words that frequently appear in both data.
        
