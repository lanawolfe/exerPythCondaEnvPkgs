# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(Need different enviornements for each project or package. Each type of project you are trying to achieve)|
|What is the default package manager in Python?            |(pip)|
|How do you manage environments and packages in Anaconda?  |(conda manages both)|
|`conda list`       |(a list of all the default packages that were installed when anaconda was installed)|
|`conda env list`       |(a list of the environments we have)|
|How do you keep your base environment unchanged?       |(by creating other environments)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(bit.ly/tryconda)|
|`conda create --name XXXX`       |(conda create --name ai37 python=3.8)|
|`source activate XXXX`       |(conda activate ai37)|
|`conda install YYYY`       |(conda install numpy)|
|channels in Conda       |(path or location that conda looks for packages we want to install)|
|`conda install -c ZZZZ YYYY`       |(pytorch pytorch)|
|`conda config --show channels`       |(shows the channels currently available)|
|`conda config --add channels ZZZZ`     |(conda-forge)|
|conda-forge.org       |(shows packages only available on this channel)|
|`source deactivate`       |(takes us back to our base enviornment)|
|`conda config --get channels`       |(tells us the priorities of the channels from highest to lowest)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#Paste your results here.
(da35) C:\Users\lwolf>conda env list
# conda environments:
#
base                     C:\Users\lwolf\anaconda64
ai37                     C:\Users\lwolf\anaconda64\envs\ai37
da35                  *  C:\Users\lwolf\anaconda64\envs\da35

```
* What command would you use to remove the environments you created for this exercise from your computer?

```
#Type the command here.
# conda deactivate conda remove -n mane ai37 --all
```
