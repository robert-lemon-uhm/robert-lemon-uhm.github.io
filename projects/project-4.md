---
layout: project
type: project
image: images/TwitterLogo.png
title: Python Tweet Classification and Generation
permalink: projects/MarkovTweetModels
# All dates must be YYYY-MM-DD format!
date: 2020-10-31
labels:
  - Python
  - Google Colab
  - Machine Learning
summary:  Three different models to classify and generate tweets from the 2020 presidential candidates from UH Manoa's ICS 235 Machine Learning class.
---

This project is a demonstration of understanding of the machine learning Markov model.  Three different models were trained on roughly 3,000 tweets from each of the two presidential candidates from the 2020 election.  The models were used to generate random tweets from each candidate, as well as classify the author of tweets in a set of testing data.  The three different implemented models are a first-order Markov model based on characters, a first-order Markov model based on words, and a second-order Markov character model.  The character models had 27 possible characters (the alphabet and spacebar), and the word model had a dictionary of around 35,000 words.

While this project was incredibly interesting to work on, it was also a great learning experience.  As I have only just been introduced to the language, this project was a great opportunity for me to practice my skills in python.  Implementing some of the default python functions from scratch also allowed me to gain a deeper understanding of what actually happens behind the scenes of this high-level programming language.  It also provided me with a clear example of how the language processing models discussed in class actually work, which helped me build a functioning understanding of machine learning as a whole.

Below is the ROC curve of the tweet classifications, which consistently had an AUROC value of over 0.98 for the first order word model.

<img class="ui image" src="{{ site.baseurl }}/images/Project4Results.png">


Below are sample tweets that have been generated from models trained on each candidate’s previous tweets (note that longer tweets have been removed since there was too much noise):

```
TRUMP: the second amendment.
TRUMP: rt @ ivankatrump!
TRUMP: yes, and the great 2nd.
TRUMP: great again, russia, dzgr
TRUMP: rt @ cnn, a russian hoax : 30 years that the virus # obliterates cnn # paycheckprotectionprogram.
TRUMP: rt @ realdonaldtrump
TRUMP: rt @ foxnews : reader tip : https : / t. co / w …

BIDEN: it again.
BIDEN: happy # fourthof6ipvy
BIDEN: president trump seems like @ teamjoe
BIDEN: over.
BIDEN: dreamers
BIDEN: joebiden will finally receive the biden record.
BIDEN: president.
```

An interesting side-note in this project was looking at the tweets that the models misclassified.  Misclassification usually occurred on tweets that one candidate wrote but were in the typical style of writing as the other candidate.  A couple examples are posted below:

```
Mislabeled Trump Tweets

RT @NationalMallNPS: In the wake of last night's demonstrations, there are numerous instances of vandalism to sites around the National Mal… (Confidence: ~100%)

RT @senatemajldr: Small businesses, working families, and medical responders across this country have made it clear: They need help now.… (Confidence: 99.99%)

“On February 19th there was a Democratic Debate, in Las Vegas. Three words weren’t said: Virus, CoronaVirus, or COVID19. NEVER came up!” @BretBaier (Confidence: 99.99%)

Mislabeled Trump Tweets

Thank you, Minnesota! https://t.co/BqKfvLOJDy (Confidence: ~100%)

RT @HaleyARing: First day of action for @JoeBiden out in Buena Vista County!!! The humidity doesn’t stop #TeamJoe and @BuenaVistaDems !! (Confidence: ~100%)

Thanks, Obama. https://t.co/kBXnvbJ9ND (Confidence: ~100%)

```


You can view the whole code for each model in the [GitHub repository](https://github.com/robert-lemon-uhm/Presidential-Tweets-Markov-Models) for this project.

