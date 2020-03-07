---
title: "Safety measure for static data models"
date: 2020-03-07
tags: DataModelling
categories: DataScience
published: true
---
Quite often data modelling involves building a model based on data retrieved from the real world. The time frame of the data may be a day, a month or even years. Usually lengthier data is better for training.

And we store the real-world data in a database and we often fall into a trap thinking data is static.

This becomes problematic when we run a model that feeds on data that is produced in real-time. 

We never know how the data would change in anytime and appropriate safety measures are required to avoid absurd behaviour of the model.

### Checking model input
Before the data goes into the model, the input data can be checked to see if it resembles a distribution of the training data used for building the model.
If the input data is far from the distribution, a model can produce an alert to inform about the unusual input data.

### Checking model output
Similarly, checking can be done with the output of the model. If the output doesn't match with the usual output distribution or expectations, then an alert can be made to inform this absurdity.

These measures can help a user to identify a change in the incoming data and engineer the model accordingly without impacting business with wrong model outputs.

### Reference
[Tugrul, K. (2020). <i>Static Machine Learning Models in a Dynamic World</i>. towards data science]

[Tugrul, K. (2020). <i>Static Machine Learning Models in a Dynamic World</i>. towards data science]: https://towardsdatascience.com/static-machine-learning-models-in-a-dynamic-world-ff1ea1b0892c
