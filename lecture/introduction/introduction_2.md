# Introductory Session II

This week, I want you to explore with you the basics of Jupyter Notebooks. In the first place, you won't have to program anything by yourself at this point. I just want you to familiarize yourself with the application so that next time, we can dive right into our first Python programming session! All I want you to do for today, is (a) to open a jupyter notebook on your computer, (b) follow me while I go through a first notebook covering some functionality of jupyter notebooks, and complete the first (very easy!) homework assignmentt. 

The things covered in this section will introduce central concepts for our subsequent endeavors in this class. More precisely, we'll explore `jupyter notebooks` as one form of interacting with your computer, specifically `python`. Getting a good hang of this will be important as most of our `python` endeavors will happen within `jupyter notebooks` and they are a staple in research workflows.


## Create an Environment and Install Python packages in conda

Before that, we want to make sure that a number of packages are installed on your system that you may need for the next sessions.

For this, we need to open a terminal (eg in PyCharm, or the bash in linux, or a terminal window on your Mac). 

Let's first have a look whether you already have an environment and what packages are installed: 

        conda env list

We can also check which packages are installed in your system: 

        conda list

Now let us generate a new environment for this course: 

        conda create -n pfp2026 python=3.13

Use the above command to check whether it indeed extists, and then activate it: 

        conda activate pfp2026

Next, let's install some of the packages we need: 

        conda config --append channels conda-forge
        conda config --set channel_priority strict
        conda install ipython jupyter jupyterlab matplotlib numpy pandas scipy seaborn pingouin statsmodels plotly

Finally, let's start jupyter notebook and have a look: 'jupyter notebook'



### Objectives 📍

- Learn how to open jupyter notebooks locally and create your own jupyter notebook
- learn basic and efficient usage of the jupyter ecosystem & notebooks


### Materials 📓

Please see the rendered version of the `jupyter notebook` [Introduction II - jupyter notebooks](https://cfiebach.github.io/Python_For_Psychologists_26-27/introduction/intro_jupyter.html) in the `ToC` on the left.


You can also download the notebook itself so that you can open it in your own browser: https://github.com/cfiebach/Python_For_Psychologists_26-27/tree/main


### Tasks for subsequent meeting 🖥️✍🏽📖

You should create a `jupyter notebook` with
- **mandatory**:  `3 different cells`:
            - 1 rendered markdown cell within which you name your favorite movie and describe why you like it via  
              max. 2 sentences
            - 1 code cell with an equation (e.g. `1+1`, `(a+b)/(c+d)`, etc.)
            - 1 raw cell with your favorite snack
- **optional**: try to include a picture of your favorite animal
- save the notebook and e-mail it to fiebach@psych.uni-frankfurt.de

**Deadline: Tuesday, November 03, 2026; 23:59h EST**


If you're eager to explore more, feel free to do so, for example [over here](https://jupyter-notebook.readthedocs.io/en/latest/notebook.html). 
