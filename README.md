# Lab 1 : Passive Network Measurement
  
For this lab, you may work solo or with one other partner of your choice.
You are not allowed to copy or look at code from other teams. However,
you are welcome to discuss the assignments with any students without sharing code.

## Team Info

Partner A: Name (UTEID)

Partner B: Name (UTEID)

(Note once the team is formed, you may not leave the team as code base is very small.)

### Check Course Calendar/Canvas for Due Dates
By **checkpoint** deadline
* Fill out the team info above and push this updated README to your team repository.
* Also make sure to submit the URL of your team repository.
* Complete `TODO 1` through `TODO 6` in `Lab1_Notebook.ipynb` and push the updated notebook (and other updated files) to your team repository.

By **final** deadline
* Complete the rest of the `TODOs` in `Lab1_Notebook.ipynb`.
* Push the updated notebook (and other updated fileds) to your team repository.

## Getting Started

On your host machine (not the VM), go to the root of the `Lab0` folder (Not `Lab1` folder but `Lab0`, the very first lab)
```
$ cd {YourOwnPath}/lab-{YourTeamNameForLab0}
$ ls
```
With the ls command above you should see `README.md` and `assignments` directory

Let's double check you have .git folder in the current directory
```
$ ls .git
```
Since we want to move on to Lab1 we will be moving .git folder to .bak folder 
so that the assignments directory can be linked to the new repository
```
$ mkdir .bak
$ mv .git .bak
```
Now your current directory is no longer associated with git.
Let's cd into assignments directory and under assignments git clone your team repository for Lab 1
```
$ cd assignments
$ git clone https://github.com/cs356-sp21/lab1-{YourTeamName}
```
You should see the starter code created under assignments/lab1-{YourTeamName}

Now let's start up the VM. Note that you are still under assignments directory where `Vagrantfile` and `cs356-sp21-minilab.box` file is.
```
$ vagrant destroy
$ vagrant up
$ vagrant ssh
```

On the VM, run the command `sudo ~/.local/bin/jupyter-notebook &`. This will
start a new Jupyter notebook server in the background. Even though it is
running in the background, it will sometimes print informative messages to the
terminal. You can press Enter each time you get a message to get the shell
prompt back. To shut down the notebook, run `fg` then press Control-C twice
(once to get the confirmation message, another time to skip confirmation).

While the notebook is running, on your host machine, open up your browser and
type `localhost:8888` in the address bar. This should open to the Jupyter
notebook file selection window.  Juypter notebook is actually running on port
8888 on your vagrant VM, but you can access it through your host machine
browser because the port is being forwarded between the VM and the host
machine.  

In the file selection window, enter the `lab1-{YourTeamName}` directory and 
navtigate to `Lab1_Notebook.ipynb` and open the notebook. 

You will see the instructions for the rest of the assignment.  Work through this notebook from top to bottom and complete the sections marked "TODO."

**Remember to "Save and Checkpoint" (from the "File" menu) before you leave the
notebook or close your tab.**  

## Jupyter Notebook

Jupyter Notebook (formerly called iPython Notebook) is a browser-based IDE with
a cell-based editor.

Every cell in a notebook can contain either code or text ("Markdown"). Begin
editing a cell by double-clicking it. You can execute the code in a cell (or
typeset the text) by pressing `shift-enter` with the cell selected.  Global
variables and functions are retained across cells. Save your work with the
"Save and Checkpoint" option in the "File" menu. If your code hangs, you can
interrupt it with the "Interrupt" option in the "Kernel" menu.  You can also
clear all variables and reset the environment with the "Restart" option in the
"Kernel" menu.

The "Help" menu contains many additional resources about Jupyter notebooks
(including a user interface tour, useful keyboard shortcuts, and links to
tutorials).

## Submission

TODO: Remember to put your names and eids in the marked location at the top of the
file. Push the updated files to the team repository.

#### Acknowledgement
This assignment is adopted from [Nick Feamster](https://computernetworksbook.com/resources.html).

# cs356-lab1-starter-python3
