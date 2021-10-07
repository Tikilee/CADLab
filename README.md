This is a very basic guide on python environment setting in CAD Lab Task and will keep updating.

# 1. Start python
* Install Anaconda  
* Install PyCharm  
we'll use PyCharm as the code IDE.  
Notice: As students, we can get PyCharm Professional version freely. Please refer to [here](https://zhuanlan.zhihu.com/p/338280181) 
if you want.

# 2. Creat new conda env
Open your terminal and try to create new environments as following steps.
* Input `conda env list` to see conda environments you own.  
* Input `conda create -n env_name python=x.x` to create a new environment(`python=3.7` is recommended). 
Once created, you can use `pip list` to show packages the env installs or `pip freeze > requirements.txt` to 
get package list txt.
* `conda activate env_name` to enter the new environment. Now use `conda install package` to install packages you want! 
Use `conda deactivate` to exit.
* If you want to package your environment, use `conda env export > env_name.yml` to export.  
  
Notice: I packed my environment `CADLab.yml` which can be found in GitHub. Try `conda env create -f CADLab.yml` to skip the
steps above and directly install the environment.

# 3. Use conda env in PyCharm
In PyCharm, `setting` -> `Python Interpreter` -> `Show all` -> `add` -> `conda environment` -> `existing environment` ->
`conda executable` -> choose one env  
You can find more detailed guide in [here](https://zhuanlan.zhihu.com/p/39542494)

# 4. Use jupyter in PyCharm
`conda install jupyter` if there not.  
Create a new .ipynb file. Now you can use it in Pycharm!