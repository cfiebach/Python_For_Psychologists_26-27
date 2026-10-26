# Setup for the course

There are a few things you need to get working on your computer in order to follow this course. However, don't worry as it's all gonna be [open source](), won't require a lot of storage and will be explained in detail.

In general getting `Python` & friends to work reliably on your machine is going to be very beneficial. This holds true for the course but also beyond. The following tools focusing on open and reproducible (neuro-/data-) science) will therefore not only be necessary for this course, but may allow you to build an "everyday" research workflow around them, for example when writing your Master's thesis. This even applies if you won't continue with `python` (we certainly hope you do) and instead work with `R` (of course also cool), `matlab` (weeeeeeeell...) or what have you. 

You'll find the (hopefully) comprehensive set of install instructions below. We first focus on just two core pieces of software, and may at later points potentially add more.   

Don't worry, you got this!

![logo](https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805)\
<sub><sup><sub><sup>https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805</sup></sub></sup></sub>


## General things

There are a few computing requirements for the course that are absolutely necessary (beyond the few software packages you should install, described below):

1. You must have administrator access to your computer (i.e., you must be able to install things yourself without requesting IT approval).
2. You should have at least 20 GB of free disk space on your computer (but we would recommend more, to be safe).
3. If you are using Windows you must be using Windows 10/11; Windows 7 and 8 will not be sufficient for this course. Note that on private computers, Windows 10 has security updates until October 2027, but at some point, it has to be upgraded to Windows 11.

If you foresee any of these being a problem please reach out to one of the instructors and enquire what steps you can take to ensure your setup is ready for the course.

## Required software

**Please wait with installation until you get a final OK from our side by E-Mail!!!**


To get the most out of the course, we ask that you to install the following software (software/things in () are not entirely necessary but definitely great to have):

- `Python 3` (see below - suggested via Anaconda)
- A remote-capable text editor, also called IDE or integrative development environment, for example  spyder (contained in Anaconda, see below), [`PyCharm`](https://www.jetbrains.com/pycharm/), or [`VSCode`](https://code.visualstudio.com)
- A `modern web-browser`. Unfortunately, macOS users may want to have a different browser besides 'Safari' (at least as of 2025), like 'Firefox' or 'Chrome'.

The primary way we suggest is to install the [`Anaconda Distribution`](https://www.anaconda.com/docs/getting-started/main). Anconda makes life quite easy: It includes python3, as well as hundreds of data science standard packages. It brings everything you need for this course - including `jupyter notebooks` and a graphical IDE, called `spyder`. After installing Anaconda, all these can be opened from a central window, the `Anaconda Navigator`. To be on the save side, you should have around 10 GB free on your computer to go this route. (To test this, I have just installed Anaconda on a 7 or 8 year old Windows 10 laptop. During installation, it asked for around 6 GB of free disk space, the Anaconda folder on my computer now has the sizee 5.05 GB.)

A more lightweight variant is the installation via [`Miniconda`](https://www.anaconda.com/docs/getting-started/concepts/anaconda-or-miniconda#miniconda). `miniconda` is a frequently used system in scientific computing that contains `python` and `conda`as package management system. It is an efficient way of keeping your software packages up to date and of managing the environment in which you conduct scientific computing (like data analysis), but does not yet include a graphical IDE or specific packages. According to the provider, it only uses around 1 GB or so on your computer (but see below). Packages that we will use have to be installed manually via the command line - but this is also not difficult. `PyCharm is a powerful user interface, in which we can run interactive python notebooks but which also provides us with a terminal window through which we can do other things like installing packages or managing our computing environment. (`spyder` provides us with the same features, if installing `Anaconda`.) 

Here is some info on the [`difference between Anaconda and miniconda`](https://www.anaconda.com/docs/getting-started/concepts/anaconda-or-miniconda). *And here is an automatically generated estimate of the storage space that our installations will require on your system:*

| OS | (a) Miniconda + PyCharm + numpy, scipy, pandas, matplotlib, seaborn | (b) Anaconda (packages included, w/out PyCharm) |
|---|---|---|
| **Windows** | ca. 2,5-3,5 GB (Miniconda ~0,5 GB + Pakete ~1 GB + PyCharm ~1-1,5 GB) | ca. 4-5 GB |
| **macOS** | ca. 2,5-3,5 GB (Miniconda ~0,5 GB + Pakete ~1 GB + PyCharm ~1-1,5 GB) | ca. 4-5 GB |
| **Linux** | ca. 2,5-3,5 GB (Miniconda ~0,5 GB + Pakete ~1 GB + PyCharm ~1-1,5 GB) | ca. 4,5-6 GB |


If you already have any of the above software tools/packages installed (what are you even doing here?), or are confident you’ll be able to install them by the time the course starts, or a have enough programming experience that you have alternative installations with similar functionality, you can use these. 

There are a number of further software that may become relevant in the next weeks, but do not have to be installed right now. These influde:

- Specific python packages, e.g., `numpy` or `scipy`. 
- `PsychoPy` stand-alone ìnstallation.
- Most likely [`Discord`](https://discord.com/) for communication purposes.
- Most likely [`Discord`](https://discord.com/) for communication purposes.
- A command-line shell: [`Bash`](https://www.gnu.org/software/bash/), already included in macOS and LINUX, and under windows probably best to use 'gitbash', which comes with the 'Git for Windows' package, see next bullet point.
- A version control system: [`Git`](https://git-scm.com/).
- A [`GitHub`](https://github.com/) account.


The rest of this page provides more detail on installation procedures if you want to use `miniconda` as Python environment, rather than `Anaconda`, with separate instructions for each of the three major operating systems (`Windows`, `Mac OS`, and `Linux`).


### Some quick general notes on instructions

- There is no difference between `Enter` and `Return` in these instructions, so just press whatever the equivalent on your keyboard is whenever one is stated
- If you already have some of these things installed on your computer that should (theoretically) be okay.
- Having multiple different `Python` installations on your computer can lead to frustrating issues that are very difficult to debug. Thus, if you have already installed `Python` via some other application (not `Miniconda`/`Anaconda`), it's strongly encouraged to uninstall it before following the instructions below. Alternatively, you should (be able to) assure that the basic needed functionality works in your setup. At the moment, this primarily involves running python interactively in jupyter notebooks.


### Installing Anaconda

Go to the [`download page`](https://www.anaconda.com/download). Choose the right side (Build with Python) but **DO NOT** click the green button (Get Started with Anaconda Distribution) but rather hit the small link below it: `Skip to download`! From here, everything should be self-explanatory.

To check if the installation works, open `Anaconda`. You should see the `Anaconda Navigator`:
```{image} static/pfep_anaconda_1_navig.jpeg
:width: 700px
:alt: Screenshot Anaconda Navigator
```

There, click on `jupyter Notebook`. Your browser should open a new window: 
```{image} static/pfep_anaconda_2_nb_browser.jpeg
:width: 700px
:alt: Screenshot jupyter Notebook in Browser Window
```


Here, select `New` > `Python 3 kernel` on the right upper corner. 
```{image} static/pfep_anaconda_3_startNB.jpeg
:width: 700px
:alt: Screenshot Start Notebook
```


A new window should open in the browser, which contains a `jupyter Notebook` with a box in which commands can be executed. Here, type `print("Hello world!")` and hit `Shift+Enter` to execute the command. You should see something like this: 
```{image} static/pfep_anaconda_4_nb_test.jpeg
:width: 700px
:alt: Screenshot Test Code
```



### OS-specific installation instructions

Select the tab that corresponds to your operating system and follow the instructions therein.

````{tab-set}
```{tab-item} Windows

**Python**

1. Go to the Anaconda website and follow the guidelines for the installation instrcutions: https://www.anaconda.com/docs/getting-started/miniconda/install#windows-installation . Please read through the following points before installing!
2. This will take you also to the download page on their website. Note: Please ignore the box on the top right that says "Download now. Get access in 30 seconds.". Rather, go to the very bottom of the download page and click the button saying 'Download Miniconda Installer'. Here, select on the right side the 'Miniconda Installer', download it and run it. 
3. The installation guideline webpage also notifies you that it makes sense to select the 'Just Me ...' option, which means that miniconda is installed into your personal user account, and that it makes sense to select the 'Create Shortcuts' option (so you will find miniconda in your start menu).
4. Please follow their suggestion to not select the option of adding miniconda to your PATH variable. For now, we will not do this.


**PyCharm**

1. Go to https://www.jetbrains.com/pycharm/ and click the download button, then run the `.exe` file.
2. During installation, you have to allow PyCharm communication with local networks, but allowing access to public networks is not recommended.
3. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
4. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 

```


```{tab-item} Linux

(Note that I did not check the LINUX installation instructions as I have no LINUX machine available, but think that these should continue to work.)


**Bash shell**

You already have it!
Depending on which version of Linux you’re running you may need to type `bash` inside the terminal to access it.
To check whether this is necessary, follow these steps:

1. Open a terminal and type `echo $SHELL`.
   If it reads `/bin/bash` then you are all set!
   If not, whenever the instructions read "open a terminal," please assume you are to open a terminal, type `bash`, and then proceed with the instructions as specified.


**Python**

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
        bash Miniconda3-latest-Linux-x86_64.sh


2. A license agreement will be displayed and the bottom of the terminal will read `--More--`.
   Press `Enter` or the space bar until you are prompted with "Do you accept the license terms? [yes|no]."
   Type `yes` and then press `Enter`
3. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`).
   Leave this default and press `Enter`.
4. When you are asked "Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no]," type `yes` and press `Enter`.
   Exit the terminal once the installation has finished.
5. Re-open a new terminal.
   Type `which python` into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
   - If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
     If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.
6. Type the following to remove the installation script that was downloaded:

        rm ./Miniconda3-latest-Linux-x86_64.sh


**PyCharm**

1. Check whether you find PyCharm in your Linux version's packlage manager. 
2. If not, here is a description of how to install a standalone version of PyCharm under Linux: https://www.jetbrains.com/help/pycharm/installation-guide.html#standalone_linux . Often, one can also find more specific descriptions for your LINUX on the internet.
3. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
4. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 



```

```{tab-item} MacOs


**Python / Miniconda**

1. There are two ways to install miniconda on macOS - one using a graphical installer (as with many other programs), one using commandline in the terminal. Both are described on the installation page of miniconda: 

https://www.anaconda.com/docs/getting-started/miniconda/install#macos-linux-installation

The commandline installation procedures are described further down under 'quickstart'. Please note that the code given there is for newer Macs that use the Apple Silicon processors (i.e., not Intel). 

2. When using the graphical installer, you will be pointed to the download page on their website. Note: Please ignore the box on the top right that says "Download now. Get access in 30 seconds." which suggests you to register with Anaconda. Rather, go to the very bottom of the download page and click the button saying 'Download Miniconda Installer'. Here, select on the right side the correct 'Miniconda Installer' (Apple Silicon vs. Intel), download it and run it. 
3. The installation guideline webpage recommends to choose the option to install for all users, which will place the program in '/opt/miniconda3'. 


**PyCharm**

1. Go to https://www.jetbrains.com/pycharm/ and click the download button.
2. Select the *.dmg Installation image that fits to your system - either Apple Silicon or Intel processor - and download it.
3. Double click the dmg file and move PyCharm into your 'Applications' folder. 
4. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
5. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 

```
````

**Note**: If the instructions aren't working and you have spent more than 15-20 minutes troubleshooting on your own, please consider visiting the office hour offered for installation support. You will have received an email specifying when this happens. 


### Python Packages

For the course, we will need a few python packages that we will add to our python installation. We will do this together in the next session. 


### Modern web browser

Install Firefox or Chrome.
(As of 2025, Safari did not work for what we plan to do.)
Microsoft Edge is not modern, despite what Microsoft might try and otherwise tell you.


Yeah, you did! Great job!

![logo](https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158)\
<sub><sup><sub><sup>https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158</sup></sub></sup></sub>


