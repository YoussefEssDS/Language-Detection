# Language-Detection (Python)
## A machine learning tool for recognizing text language with Python.

  This is an attempt to create a machine-learning based program. This program has for a purpose detecting the language of a given text via a task known as Natural language processing.
  This is the first step towards creating systems capable of providing many interesting services such as: a refined automatic translation, an emproved web search in terms of relevance, and also better performance for sentiment analysis tools.
  
  So, in this project I will use data from: http://www.statmt.org/europarl/ this website provides a massive datasets for many languages. Actually each file contains the speeches held at certain european parlement session. To keep things simple I will only select 4 languages to be our targets: French, Spanish, Italian & Portuguese.
  
  So the idea is that after finishing this program, it'll be able to recieve a text, and give accurate prediction of its language. 
  
This is done, by taking into consideration that we only will train our model(s) on 4 languages. 

I will use neural networks, to train this model.

## Prerequisites:
  
  For this project I will use several libraries that are not initially installed with python. So in this section, I'll provide an extensive list of all tools needed for this project.
  
1-Pickle: A tool to dump python objects, it comes in handy looking at the big size of our datasets. Throught the code I explained the many advantages it provides, and the different problems that comes with it, and how to tackle them. Luckily, the pickle module is part of the standard library in Python for a very long time now so there is no need to install it.

2-Sklearn: Is a free software machine learning library for the Python programming language. We will use a specific modulewhich provides multi-layer perceptron classification known as MLPClassifier.
 
Easly installed using pip:

> pip install numpy

> pip install scipy

> pip install sklearn


## Realization:

  I provided a very detailed and commented code to address this project, which I devided into many Jupyter notebooks to gain in visibility and performance (large dataset) by processing each language seperatly. 
  
  I tried many configurations for fitting the models, and I finally approved on two models: The first that was fit using Quasi-Newton method and reached a cross-validation test accuracy estimate of 85%. The other model fitted using the stochastic gradient-based optimizer proposed by Kingma, Diederik, and Jimmy Ba managed to achieve a 99% cross-validation test accuracy estimate. Although I kept the two since I doubted the second for overfitting. After testing the program on new texts. I noticed that with texts long enough, both models can provide accurate predictions of the text language.


## Test:

![capture](https://user-images.githubusercontent.com/47015407/51806919-e7632d80-2277-11e9-9cf2-980c542e2b61.PNG)

## Sources:

1- https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html#sklearn.neural_network.MLPClassifier

2- https://scikit-learn.org/stable/modules/neural_networks_supervised.html

3- https://pythontips.com/2013/08/02/what-is-pickle-in-python/




  
