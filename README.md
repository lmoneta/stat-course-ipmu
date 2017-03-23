# Notebooks for the IPMU Course : *Practical Statistics for Particle Physics Analyses* 

This is the git repository containing the notebooks for the IPMU statistics course given by L. Moneta and L. Lyons. 
The agenda of the event is at 

http://indico.ipmu.jp/indico/event/119/


The hands-on session of the course consists of Jupyter notebooks which can be run on the CERN SWAN service ( https://swan./cern.ch )


## Getting the repository

First thing to do before running the tutorial notebooks is to clone the git repository. The course should be run on SWAN, where dedicated accounts will be provided.
n a nutshell, "SWAN (Service for Web based ANalysis) is a platform to perform interactive data analysis in the cloud". It gives you access to the LCG software stacks and to your CERNBOX files. 

* If you have a CERN account already you can use it for the course. You need to have an active **CERNBOX** to use Swan.
If you have never used CERNBOX before, you need to just login in (https://cernbox.cern.ch/).

* If you don't have a CERN account, please contact  me directly and a temporary accounts is made available for the course. CERNBOX shoukld be activated in these account. In case it is not you will get
  an error connecting to SWAN. In this case please login first at https://cernbox.cern.ch/ 


If you have a local ROOT installation with Python enabled and you have installed also the python Jupyter and Metakernel packages you can run the notebooks locally on your computer, by typing
`root --notebook`
In this case you can go directly to the 5th item.  

### Instructions for SWAN: 

1. Connect to SWAN ( https://swan./cern.ch )
2. Select **Go to my Notebooks**
3. Customize SWAN by using the default **88** software stack version or the **Development  Bleeding Edge**. The development version is reccomended if you intend to run some notebooks in Python.
4. Select **Start My Session**
5. Create a  **Terminal** window, by using the **New**  command in the top right corner
6. Clone the git repository by typing
`git clone https://github.com/lmoneta/stat-course-ipmu.git`
7. Go back to the previous browser window (SWAN Home) and select the `stat-course-ipmu` directory. The notebook will be now visible
8. Select the desired notebook

## Swan and Jupyter notebooks quick start ##

If you never used jupyter notebooks, you can find some quickstart information at the following links [What is a jupyter notebook?](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/What%20is%20the%20Jupyter%20Notebook.ipynb), [Notebook Basics](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Notebook%20Basics.ipynb),  [Running Code](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Running%20Code.ipynb).

For more information on SWAN, see the swan website: https://swan.web.cern.ch

* If you think think the Jupyter notebook is stuck, open a terminal on swan and execute `top`: if the cpu is not being used (0%) by any of your processes, you may have to restart the Jupyter
kernel.

* There is a known issue when executing `import ROOT` in a Python notebook, which may get stuck.  However this problem should not be present anymore with the latest development version of SWAN.


**IMPORTANT:**    
* Please only have one notebook at the time on swan (you have to select the "running" tab and shutdown the notebook when done)
* Please avoid Chrome, it has known problems restarting kernels.
* Try to avoid performing expensive computations: *swan is meant for fast prototyping*. 
     * Each swan container has 2 GB of ram assigned, and only one core assigned



