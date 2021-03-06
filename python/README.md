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
- What is **Anaconda**? You'll get to read all about it in **Part 2** (feel free to take a look at the first paragraph of Part 2 below now or later).
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
    ![image_01](https://user-images.githubusercontent.com/1342429/87240116-6a1b7200-c3b2-11ea-98d8-c1398e73bbbb.png)

### Part 2. Create a Conda environment
- What exactly is **Conda** and how does it differ from **Anaconda**? **Conda is a software (package) manager and an environment manager**, whereas **Anaconda is a software distribution**, which is just a fancy way of saying that it's **a collection of different software bundled together**. Anaconda's main purpose is to make it easier for data science and machine learning practitioners to get started building something. Conda, on the other hand, can create different environments (essentially different folders on your machine) and install different software to those environments. Without Conda or some other type of environment manager, you would run into a lot more issues trying to install or run various software, which might require different or older versions of some other software before they can run successfully. Conda makes it much easier to switch between different versions of Python, for example (versions 2 and 3 are very different).
1. With the Anaconda Navigator still open, let's click on the Environments tab in the left sidebar, below Home.
1. In the bottom left corner, click the Create button. Python 3.7 should be selected by default. Let's name our environment `python-ml` and click Create. You should see on the right that Anaconda has installed some default packages that come with your newly-created environment.
    ![image_02](https://user-images.githubusercontent.com/1342429/87240124-828b8c80-c3b2-11ea-9134-9438624695e4.png)
1. Now let's click back on Home in the leftmost sidebar.

### Part 3. Install Jupyter Notebook
- What is **Jupyter Notebook**? Jupyter Notebook is software that runs in your browser and serves the purpose of a physical notebook. It differs from the way programmers traditionally write code in that every single section or "cell" of the notebook can execute your code and print results, even if you didn't specifically tell the program to write something out to screen. These "code cells" that contain Python code can also be turned into "Markdown cells." **Markdown** cells allow you to write Markdown, which is a markup language (essentially, this means it allows you to format text, as you would when writing in a physical notebook by writing hyphens for lists or underlining/starring things as headers).
- But how do programmers traditionally write code? Normally, programmers would write all of their logic in one or multiple files and then manually have to run their programs, which takes extra steps. With Jupyter Notebook, however, it's much faster to iterate on small snippets of code at a time, so that we can see what's going on with our program before moving on to the next few lines of code. To run a code cell, you can simply press Shift+Enter to execute the code and see what happens.
- Why does it seem that a lot of people in data science and machine learning like Jupyter Notebook? The steps taken from problem to solution in data science or machine learning are often long and tedious -- so very many steps that it's incredibly easy to make a mistake without checking the output, without stopping to see what's going on with a line of code before moving on. Therefore, Jupyter Notebook makes it easy to experiment, to "check our work" when it comes to writing code for data science and machine learning. Eventually, these same people might move their code from Jupyter Notebook to Python scripts (files ending in `.py`) before using the code in a real-world scenario.
- For clarity, the term "Jupyter Notebook" or "Jupyter" is in reference to the name of the software itself. When we talk about "Jupyter notebook" with a lowercase "n," we're simply referring to any notebook that you create or use from the "Jupyter Notebook" or "Jupyter" software. Thus, a "Jupyter Notebook notebook" is akin to saying "Campbell's® Soups soup."
1. With the Anaconda Navigator home page still open, in the top left-hand corner, select `python-ml` from the dropdown menu if it's not already selected.
1. We should already see Jupyter Notebook on the home page, with an Install button right beneath it. Let's click on the Install button for Jupyter Notebook.
    ![image_03](https://user-images.githubusercontent.com/1342429/87240157-ced6cc80-c3b2-11ea-92af-bafed11d5d7a.png)
1. After Jupyter completes installation, we should see it on the home page with a Launch button (instead of an Install button). Let's now click on the Launch button. In the process, you'll see a terminal window open (Mac by default comes installed with the Terminal application) that will launch Jupyter by running some code and opening up a new browser tab in your default browser.
1. You should now see http://localhost:8888/tree open in your browser, along with different folders in your home user account, such as Applications, Desktop, Documents, and Downloads.
    ![image_04](https://user-images.githubusercontent.com/1342429/87240184-f037b880-c3b2-11ea-892b-9a0dcfa53aa5.png)

## Project Setup
- What is the **Terminal** application? The "terminal" or "command line" is another way for us to access the contents of our computer, without any visual cues other than lines of text. There's no concept of clicking around. To mimic what we do on a computer, we need to type **commands** to tell the terminal or command line what to do. For example, typing `ls` in the terminal will show you a **list** of folders in your current folder. While you're using the terminal, note that **you're always in a folder** (as if you have the Finder application open on your Mac).
- How else can I access the terminal or command line? The Terminal application on Mac is not the only way. There are other software that exist to allow you to access your computer via the terminal or command line. [iTerm2](https://www.iterm2.com/) is one example that allows even more customization of your terminal.
- Why do we need terminal or command line access? We won't be learning much about the terminal or command line, other than the most basic commands. But we need to use it in this tutorial because that's the only way (at least that we know of) to **set your Conda environment in a Jupyter notebook**.
1. First off, let's launch the Terminal application on the Mac. If it's already running, let's quit it by clicking on Terminal in the very top left of your screen and selecting Quit Terminal (or you can type CMD+Q as a shortcut). Click the Terminate button if you're asked to terminate running processes in the window. Now let's launch the Terminal application again.
1. After the Terminal app is open, you'll see a window that you can type in. You might see the term `base` next to the prompt (the **prompt** is called a prompt because we can think of it as prompting you for your input). `base` is the default Conda environment; however, we want to switch to the environment we created. But first, let's learn some basic terminal commands.

### Part 1. Learn basic commands
1. As mentioned before, we're always in a folder/directory whenever we're using the terminal or command line. Let's "print working directory" (meaning, print the current directory we're in) by typing the command `pwd`. You should see something like `/Users/your_user_name` as the output.
1. Type `ls` to "list" the contents (more files and folders) of the folder that we're in.
1. We can create a new folder ("make directory") by typing `mkdir python_projects`, where `python_projects` can be anything that you want to name the folder.
1. Now let's navigate to the new folder ("change directory") by typing `cd python_projects`. (Again, replace `python_projects` with the name you actually gave the folder.)
1. Later, you can repeat these steps as many times as you need to, to create folders within folders if you wish. And if you want to go to a parent folder at any time, you can type `cd ..` to do so. But for now, let's remain in the `python_projects` folder.
1. Here are a few more common commands you can try later on your own: [view commands](https://scotch.io/bar-talk/10-need-to-know-mac-terminal-commands).

### Part 2. Download the project
1. While leaving the terminal open, visit https://github.com/hawaiiwomenintech/WorkshopMaterials in a browser.
1. Click on the green Code button and click on Download ZIP.
1. Open that zip file so that we have the uncompressed contents. You should now see a folder called "WorkshopMaterials-master" in your Downloads folder.
1. Back in your terminal, type `open .` to open up the current folder that we're in (note that the `.` stands for the current folder).
1. You can now drag the "WorkshopMaterials-master" folder into the `python_projects` folder. Let's rename "WorkshopMaterials-master" to simply "WorkshopMaterials" and close the `python_projects` Finder folder.
1. Back in our terminal, if we type `ls`, we'll see the folder.
1. Let's type `cd WorkshopMaterials` to navigate to the folder and type `ls` to see a `python` folder.
1. Let's type `cd python` to enter the folder and type `ls` to see a `README.md` and `regression_pytorch.ipynb`.
1. We're almost ready to work with the notebook! But first, let's learn some important Conda commands.

### Part 3. Learn Conda commands
- So what's the point of using the terminal and using Conda (via the command line) over the Anaconda Navigator? Well to be honest, we don't know a lot about that. It might be possible to do in Anaconda Navigator whatever we need to do via Conda, but we weren't successful looking up how to do so. So please feel free to look up how to do the equivalent in Anaconda Navigator later if you wish. For us, we find that the terminal is much faster and more convenient, as far as switching between environments and installing packages goes.
1. Let's first create a Conda environment: `conda create --name some-env python=3.7`. (`some_env` is the name of our environment.) Press `y` if you're prompted to proceed.
1. To activate the new environment, let's type `conda activate some-env`. You should now see that `base` has changed to `some-env` in the prompt.
1. From here, anything that you install will only belong to this one environment called `some-env`, nothing else. It would not affect anything you install in the `python-ml` environment that we created earlier. But for demonstration purposes, let's exit this environment (say, we no longer want to work with it) by typing `conda deactivate`. The prompt should now say `base` again.
1. To delete an environment (along with everything that you installed within it), let's type `conda env remove --name some-env`.
1. Now let's see what environments we have: `conda env list` (note that the * indicates what environment is currently activated).
1. Let's finally switch to `python-ml` by typing: `conda activate python-ml`.
1. For more Conda commands that you can try out later: [view commands](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf).

### Part 4. Install `nb_conda` and PyTorch
1. Let's install our very first package called `nb_conda` by typing: `conda install nb_conda`. (This package makes it much easier to work with different Conda environments within Jupyter Notebook, eliminating future manual steps we'd need to take otherwise. So if you ever need to create another Conda environment, don't forget to install this too if you're going to work with Jupyter Notebook!)
1. Let's install PyTorch: `conda install pytorch -c pytorch`.

### Part 5. Launch Jupyter Notebook from the terminal
1. Now let's start Jupyter Notebook from the terminal by typing: `jupyter notebook`.
1. After a new browser tab opens, we should see the README and the PyTorch regression notebook. Let's click on the regression notebook.
1. If you run into an error with "Kernel not found," select the `python-ml` environment from the dropdown (the full name might look like "Python [conda env:python-ml]"), and then click the blue Set Kernel button.
1. You should now be in the notebook and see the Conda environment name in the top right-hand corner (under the full name, as mentioned earlier). Your Python packages (such as PyTorch) should also be available so that when you run the first code cell, you shouldn't face any errors.
1. Future note: If you ever need to quit Jupyter Notebook (don't forget to save first!), go back to the terminal and press Ctrl+C. You'll then be prompted with "Shutdown this notebook server (y/[n])?", to which you should type `y` for "yes"

## Using Jupyter Notebook
1. Try running each cell in the notebook by pressing Shift+Enter
1. Here are some Jupyter Notebook cheatsheets: [jupyter_cheatsheet_1](https://www.edureka.co/blog/wp-content/uploads/2018/10/Jupyter_Notebook_CheatSheet_Edureka.pdf) and [jupyter_cheatsheet_2](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Jupyter_Notebook_Cheat_Sheet.pdf)
