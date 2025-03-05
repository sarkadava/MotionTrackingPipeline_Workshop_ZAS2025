# Workshop: How to build your motion tracking pipeline

This repository stores all materials for a workshop on **How to build your motion tracking pipeline** which takes place on the 12th and 13th of March at ZAS (Berlin).

## Get ready

### Step 1: Installing Python

To be able to follow the workshop and explore the coding procedures of building a motion tracking pipeline, you will need to have a Python available. 

The easiest way to get Python is installing [Anaconda](https://www.anaconda.com/download), a common platform for this programming language.

> ["!IMPORTANT"] 
> At some point during the installation process, you need to check that you want **to add Anaconda/Python to system path**. Without that, your command prompt or the text editor will not know where to find executor. 

If you feel you need a guidance, you can follow one of many tutorials online (e.g., [here for Mac]( https://www.youtube.com/watch?v=YJC6ldI3hWk), and [here for Windows](https://www.youtube.com/watch?v=UTqOXwAi1pE)). 

### Step 2: Get yourself a fancy text editor

To work with Python scripts, it is very convenient to have a text editor. Essentially, this can be any software that can edit texts, but I personally recommend - and for this workshop highly encourage - to use [Visual Studio Code](https://code.visualstudio.com/).

Once you have install it, you need to do few more adjustments so that VS Code can recognize a Python script. Go to Extension panel (*Ctrl + Shift + X*) and search for Python. Click on the install button, et voilà! 

> [!TIP] 
> One of the reasons why VS Code is really nice lies in the extensions. One of my favorites is [Data Wrangle](https://code.visualstudio.com/docs/datascience/data-wrangler) that allows you to look through your dataframe in much more friendly way than, for instance, RStudio (no hate though :angel:)

### Step 3: Clone/download the repository

Once you are all set up, it's time to get this repository to your PC.

Here, you can either use [Github Desktop](https://desktop.github.com/download/) which will later also allow you to synchronize your local version of this repository with any updates I may do here.

> [!NOTE] **How to clone repository via Github?** After installing, launching Github Desktop, and signing in with your Github credentials, simply click on *File > Clone repository... > URL* and paste there the link to this repository, https://github.com/sarkadava/MotionTrackingPipeline_Workshop_ZAS2025

If you don't want to install yet another software, you can just download the repository. At the top of this page, click on **<> Code** and then **Download ZIP**. This will download the repository.
![alt text](image.png)

### Step 4: Prepare your environment

During the workshop, we will work with so-called *virtual environment*. I will not go into detail, but environment essentially make sure that our project is safely isolated from the rest of the Python packages and certain versions therefore do not collide.

Now turn on your Anaconda Prompt and type

```
cd C:/Directory/where_the_downloaded/folder_lives
```

> [!CAUTION] 
> If you are a Mac user, you might notice that there is nothing like Anaconda Prompt to be found. You can simply use your Terminal.

Now it's time for our environment. You can create one by typing

```
conda create --name MTworkshop python=3.12
```

and then activate it with

```
conda activate MTworkshop
```
You should now see (MTworkshop) in the beginning of your line. 

Finally, we want to install some packages that I have prepared into the *requirements.txt* file. In your prompt, type

```
pip install -r requirements.txt
```

### Step 5: Verify that it worked

Now you can open your Visual Studio Code, click on *File > Open Folder* and select the folder where this repository lives. In the right panel, you shoul be able to see all the files. Click on the jupyter notebook Test.ipynb

Click on the play button. A window will pop up to select a kernel source. Click on *Select Python Environment* and now choose the one we have created a second ago, *MTworkshop*. Now click on the play button once more.

The moment of truth has come. If nothing screams red and a welcome message got printed, congratulations, you are ready to go! :blush:



