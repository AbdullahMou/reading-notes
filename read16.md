# Data Science Primer
##  Bird's Eye View 

### machine learning

**Machine learning** is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.

### Key Terminology

* **Model** - a set of patterns learned from data.
* **Algorithm** - a specific ML process used to train a model.
* **Training data** - the dataset from which the algorithm learns the model.
* **Test data** - a new dataset for reliably evaluating model performance.
* **Features** - Variables (columns) in the dataset used to train the model.
* **Target variable** - A specific variable you're trying to predict.
Observations - Data points (rows) in the dataset

## Exploratory Analysis

* **The purpose** of exploratory analysis is to "get to know" the dataset. Doing so upfront will make the rest of the project much smoother, in 3 main ways:

  * You’ll gain valuable hints for Data Cleaning (which can make or break your models).
  * You’ll think of ideas for Feature Engineering (which can take your models from good to great).
  * You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

##  Data Cleaning
* There is no right way or technique for data cleaning, it depends from dataset to dataset
* Proper data cleaning can make or break your project, because in machine learning better data beats fancier algorithms.

  * Remove unwanted observations which includes duplicate or irrelevant observations.
  * Find and fix structural errors.
  * Filter unwanted outliers
  * Handle missing data (it is important to know that you cannot simply ignore missing values in your dataset. You must handle them in some way for the very practical reason that most algorithms do not accept missing values.)

## Feature Engineering

* Feature engineering is about creating new input features from your existing ones.
* Using your own or others expertise about the domain can will allow you to engineer informative features

  * Can you create any interaction features that make sense
  * Combine sparse classes (those that have fewer total observations)
  * Add dummy variables
  * Remove unused features  

## Algorithm Selection:

* Simple linear regression models fit a "straight line" (technically a hyperplane depending on the number of features, but it's the same idea). In practice, they rarely perform well. We actually recommend skipping them for most machine learning problems.

* Their main advantage is that they are easy to interpret and understand. However, our goal is not to study the data and write a research report. Our goal is to build a model that can make accurate predictions.

* In this regard, simple linear regression suffers from two major flaws:

  * It's prone to overfit with many input features.
  * It cannot easily express non-linear relationships.

* These flaws can be fixed by the following:

  * Regularization.
  * Using Regularized Regression Algos.
  * Using Decision Tree Algos.
  * Using Tree Ensembles.  

## Train ML Models


* It might seem like it took us a while to get here, but professional data scientists actually spend the bulk of their time on the steps leading up to this one:

  * Exploring the data.
  * Cleaning the data.
  * Engineering new features.
