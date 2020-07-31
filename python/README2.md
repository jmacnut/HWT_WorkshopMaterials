# Learning to Code in Python

Welcome to our "Learning to Code in Python" series! This is the material we'll work with for our Python meetups.  

This README2.md file is for the second session of the series.  You can also visit [README.md](https://github.com/hawaiiwomenintech/WorkshopMaterials/blob/master/python/README.md) for the first session materials.

## Learning to Code in Python Part II: Simple Linear Regression using Pytorch

The second session will focus on doing a hands-on data analysis, and we will start with a simple linear regression.
If you don't have a python project environment set up on your computer, don't worry. we will provide few online tool options. 

We plan to go through the following:
- Launching the python project environment
- Going over a brief intro to regression analysis
- Running a simple regression analysis in a simple way
- Running a regression analysis in a data science way

## Getting started
Download the session materials at https://github.com/hawaiiwomenintech/WorkshopMaterials

Join the HaWT Slack "chatting room" at https://hawaiiwomenintech.herokuapp.com/

## Launching the python project environment

### Online Resouce
[Kaggle](https://www.kaggle.com) provides a jupyter notebook workspace (and more!). To save your work, you need to create an account and it's free. (highly recommended)
  - https://www.kaggle.com/sundancefish/v1-regression-pytorch2
  - https://www.kaggle.com/sundancefish/v2-regression-pytorch-normalization

  
  
### On your device
If you have a jupyter notebook and python conda environment already set up on your computer, start your jupyter notebook.
- Launch jupyter notebook from anaconda
- In terminal type `jupyter notebook`

To start conda virtual environment   `conda activate [YOUR ENV NAME]`


## Regression Analysis
* **/python/codes/V1_regression_pytorch2.ipynb** Running a simple linear regression analysis 
* **/python/codes/V2_regression_pytorch_normalization.ipynb** Normalizing data, Training/validating datasets, Learning rate, prediction

## References

- **PyTorch:** An open source machine learning framework that supports training on GPUs and uses tensors. One of the two most popular deep learning frameworks right now (the other is TensorFlow). https://pytorch.org
- **Linear regression:** An approach to modeling the relationship between a dependent variable and one or more explanatory variables. Simple linear regression = one explanatory variable. Commonly used in predictive analysis. Basically, you've got a bunch of data points, now draw a line in the middle of them. Use that line's equation to predict where new points should go in the space. Now your job is to find the slope and intercept (weight and bias, respectively). https://en.wikipedia.org/wiki/Linear_regression
- **Neural network:** A set of algorithms loosely modeled after neurons in the human brain, designed to recognize patterns. Can have variable numbers of neurons (one to billions) and one or more architectures mixed in (convolutional, recurrent, attention). https://en.wikipedia.org/wiki/Artificial_neural_network
- **Training a neural network:** Run examples through the network, calculate the loss between the actual answer and the predicted answer, then [backpropagate](https://en.wikipedia.org/wiki/Backpropagation) that loss through the network, updating the weights with the gradients calculated in backpropagation. This is how the network learns.
