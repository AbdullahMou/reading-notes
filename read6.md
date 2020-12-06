# Random Module

![](https://i.pinimg.com/236x/79/86/28/7986285801c4cc1b1c0987a4a0ead938.jpg)

## When to use it
* We want the computer to pick a random number in a given range Pick a random element from a list, 

## Random functions
* Randint
  * `import random`
`print random.randint(0, 5)`

* Random 
  * `import random`
`random.random() * 100`

* Choice
  * `import random`
`myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]`
`random.choice(myList)`

*   Shuffle
  * `from random import shuffle`
`x = [[i] for i in range(10)]`
`shuffle(x) `

* Randrange
  * `import random`
`for i in range(3):`
 `   print random.randrange(0, 101, 5)`

# Risk Analysis

*  the process of identifying the risks in applications or software that you built and prioritizing them to test.
*  After that, the process of assigning the level of risk is done.
* The categorization of the risks takes place, hence, the impact of the risk is calculated.

![](https://risk-engineering.org/static/img/thumb-data-analysis.png)

## Why use Risk Analysis?

* In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks.

* the possible risks that you could encounter
  * Use of new hardware
  * Use of new technology
  * Use of new automation tool
  * The sequence of code
  * Availability of test resources for the application

* tackle the situation with care
  * Conduct Risk Assessment review meeting
  * Use maximum resources to work on high-risk areas
  * Create a Risk Assessment database for future use
  * Identify and notice the risk magnitude indicators: high, medium, low

## Risk Identification

* There are different sets of risks included in the risk identification process
  * Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

  * Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.

  * Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

  * Software Risks: You should be well versed with the risks associated with the software development process.

## Risk Assessment

* In the risk analysis process, these steps prove to be the most important one. It is said that this step is way too complex and should be tackled with the utmost care. After risk identification, assessment has to be dealt programmatically.

![](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Picture1-768x422.png)

## The perspective of Risk Assessment

* Effect
  * To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.

* Cause
  * To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

* Likelihood
  *  To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.

## How to perform Risk Analysis

* Searching the risk

* Analyzing the impact of each individual risk

* Measures for the risk identified
