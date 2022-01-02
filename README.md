# Programming-project

This repository is submitted as partial fullfillment of a H.Dip in Data Analytics in Computing

*G00398250 Katie O'Brien*

***

This repository contains one Jupyter notebook, an images and dataset folder and a requirements.txt which should not be modified as it contains important configuration files which Binder requires to run correctly.




## System Requirements 
***


To modify or run the notebook on a local machine requires the latest version of Python. Anaconda is an easy to use version available at the following  [url](https://www.anaconda.com/) for Windows, Linux and Mac. Alternatively the static and interactive web based versions of the notebooks are available via the links below. 

## Running Jupyter notebook

To run the notebook on a local machine following the installation of `python` you should do the following:

1. Open the command line on your machine. I recommend [CMDer](https://cmder.net/) if using Windows, but the native terminal works fine on Linux/Mac.

2. Navigate to the appropriate folder that contains the downloaded notebook `Project.ipynb`

3. Type "Jupyter lab" and press "Enter"

4. At this point your browser should automatically start, however, if it doesn't you can copy and paste the info outputted in the terminal into the browser you wish to use and this should start the notebook.


<br>

# Project Notebook

This notebook investigates the synthesisation of data, either from a new set of variables; or an existing dataset. For this notebook I used the ```palmerpenguin``` dataset as a basis for this new data. While the Machine Learning aspect of data synthesis focused on one particular breed of penguins in the dataset, the user is invited to modify the code to run their own simulated data on the other breeds and variables in the dataset if desired.  

```
X= gentoo_male

# Fit a kernel density model using GridSearchCV to determine the best parameter for bandwidth
bandwidth_params = {'bandwidth': np.arange(0.01,1,0.05)}
grid_search = GridSearchCV(KernelDensity(), bandwidth_params)
grid_search.fit(X)
kde = grid_search.best_estimator_

# Generate/sample 100 new rows from this dataset
ai_male = kde.sample(100, random_state=rand_state)

```





### Static link
The static view for this notebook on nbviewer is available at:
https://nbviewer.org/github/kaob1991/Programming-project/blob/main/Project.ipynb 

or by clicking the following image: [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/kaob1991/Programming-project/blob/main/Project.ipynb)


### Interactive link 
The interactive link for this notebook which will open on Binder can be found by clicking the following image/URL:

https://mybinder.org/v2/gh/kaob1991/Programming-project/HEAD
or  

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaob1991/Programming-project/HEAD)

<br>










## Credits


### Project
I used  the  following resources significantly in the creation of the Project notebook: 
- `matplotlib.pyplot` - the documentation can be found below:
https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.html

- `seaborn`- further information can be found at the link below:   
https://seaborn.pydata.org/

- `palmerpenguins` Can be found at the following repository: 
 https://github.com/allisonhorst/palmerpenguins

- `pandas` - which can be found here: https://pandas.pydata.org/


- `numpy`- documentation at the following link: https://numpy.org/doc/stable/index.html

- `sklearn` ML library at the following link: https://scikit-learn.org/stable/



All addditional resources used are referenced at the end of the Notebook 


## Contact: 

Any questions/comments feel free to contact the creator on G003980250@gmit.ie
