# Learning to Code in Python

Welcome to our "Learning to Code in Python" series! This is the material we'll work with for our Python meetups. The first one is coming up on July 16, 2020.

## Learning to Code in Python Part I: Python Environment Setup

Our first session will focus on the Python environment setup that is most commonly used for data science and machine learning. We'll be installing [Anaconda](https://docs.anaconda.com/anaconda/install/#requirements), [Jupyter Notebook](https://jupyter.readthedocs.io/en/latest/content-quickstart.html), and [PyTorch](https://pytorch.org/get-started/locally/). We plan to go through the following:

- Making sure everyone has Python on their computer
- Downloading and installing [Conda](https://docs.conda.io/en/latest/)
- Creating a Conda environment
- Installing PyTorch with Conda
- Starting and using a Jupyter notebook

The Jupyter notebook will contain [code from this tutorial](https://medium.com/biaslyai/pytorch-linear-and-logistic-regression-models-5c5f0da2cb9), which we don't plan to cover line by line until our future session, Part II. But feel free to take a look at the tutorial ahead of time.

## Getting Started: Installation
- Let's follow each part below, in order, so that we can get to the fun part -- to learn about Python and PyTorch using a Jupyter notebook!
- Note that the steps below were tested on a machine running macOS Catalina version 10.15.5. If you run into any issues, try to paste any error messages that you encounter into Google and see if others have encountered the same problems. Also please don't hesitate to ask us on Slack or on meetup.com! It's possible that you'll have to change a few steps here and there when installing on Windows or Linux.

### Part 1. Install Anaconda
1. Let's follow the install instructions for Mac here: https://docs.anaconda.com/anaconda/install/mac-os/, following only the instructions under the "macOS graphical install" section -- let's disregard anything under the "Using the command-line install" section.
    - For Windows, follow: https://docs.anaconda.com/anaconda/install/windows/
    - For Linux, follow: https://docs.anaconda.com/anaconda/install/linux/
1. Click on the `macOS installer` link in step 1 of the document and click on the Download button at the top, beneath "Your data science toolkit." The page will scroll down to the very bottom, where you should select the "64-Bit Graphical Installer (442 MB)" beneath "MacOS" for "Python 3.7." Continue by clicking Save (saving it to your Downloads folder is fine).
1. Click on the `.pkg` file you just downloaded, Open it, and click Continue if prompted with "This package will run a program to determine if the software can be installed."
1. Within this document, let's continue with steps 4 and onwards https://docs.anaconda.com/anaconda/install/mac-os/, taking note of the following:
    - Click a series of Continue and Agree buttons
    - Skip step 6 in this document, as we'd prefer to install Anaconda in the default location
    - Skip step 8 as well (by clicking Continue), since we're not going to install PyCharm
    - Upon step 9, click Close to hide the installer window; it's also totally fine to click "Move to Trash" as we won't be needing the installer itself anymore
    - For step 10, follow the "macOS" step under the "Anaconda Navigator" section -- let's ignore the "Conda" section
1. Following through on step 10 of the installation document, you can open the Anaconda Navigator by pressing CMD+Space on your keyboard, which will open up Spotlight Search. Type in "Anaconda Navigator" and press Enter to open it on your Mac.
1. Feel free to deselect the checkbox "Yes, I'd like to help improve Anaconda" and then click "Ok, and don't show again."
1. Since Anaconda Navigator is now open on your Mac, you have successfully installed Anaconda!

### Part 2. Install Jupyter Notebook
- For clarity, the term "Jupyter Notebook" or "Jupyter" is in reference to the name of the software itself. When we talk about "Jupyter notebook" with a lowercase "n," we're simply referring to any notebook that you create or use from the "Jupyter Notebook" or "Jupyter" software. Thus, a "Jupyter Notebook notebook" is akin to saying "Campbell's® Soups soup."
