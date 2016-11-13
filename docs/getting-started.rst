Getting started
===============

This document describes elements necessary to perform 3FUC trajectory analysis. Trajectory was obtained running molecular dymnamics simulation in Amber package.

Analysiswas performed using gromacs tools, mdtraj package and self written python code.

Full access to the data and scripts requires Linux machine with gromacs and vmd installed (or equivalent 3D visualization tool). Additionally Jupyter notebook or Jupyter Lab to use and test codebase from ``.ipynb`` files.

Creating Virtual Environment
----------------------------

To get all python packages correct versions and depencencies use virtualenv package to create new python2 clean environment in the root folder of analysis. You must have python2 with virtualenv package already installed ::

    virtualenv venv


Activate environment by::
    
    source venv/Scripts/activate


After that use package manager to install dependencies listed in ``requirements.txt``::
    
    pip install -r requirements.txt


Check your ``.gitignore`` file if all unnecessary folder are included (along with  our virtual environment root, which may substantially grow during analysis).


Commence source tracking software (we will use git)::
    
    git init
    git add --all
    git status #(to check what changed in your repository)
    git commit -m "Initial commit, with getting-started documenttion."

You can also make remote repository to host our project files (GitHub, GitLab, BitBucket), but you need account. Once you have it create repository online and add it to your local git folder.::
    
    git remote add origin https://github.com/user/trajectrory_analysis.git
    git push -u origin master
