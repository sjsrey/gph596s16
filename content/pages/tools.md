Title: Software Installation
status: hidden


### Software Requirements

For the course we will require the following packages be installed

- PySAL 1.11.0
- SciPy
- Numpy
- iPython 
- ipywidgets
- jupyter
- matplotlib
- pandas
- folium
- cartopy

There are a number of ways to install PySAL and these dependencies. For the course, if you do not yet have the dependencies installed we suggest using one of two scientific Python distributions (below). These have the advantages of including most of the dependencies for PySAL as well as PySAL itself. Moreover, both allow for updating PySAL to the most recent release  (1.10 released July 31, 2015) which is more current that what is listed in either distribution. Both of these distributions also allow for installation of additional dependencies.

#### PySAL via Anaconda Python Distribution

1. Install [Anaconda Python Distribution][Anaconda]
2. Open a terminal (Mac or Linux) or Powershell (Windows)
2. `pip install -U pysal`
3. `pip install -U folium`

#### Creating a Custom Conda Environment

If you already have Anaconda installed and you did not want to modify your default environment, you can create a *custom conda environment* for this session using the following commands:

1. `conda create -n pysal110 scipy matplotlib jupyter ipython pandas ipywidgets`
2. `source activate pysal110`
4. `pip install -U pysal`
5. `pip install -U folium`

When you are done working in this environment, you can get back to your default environment with:

 `source deactivate`


#### PySAL via Enthought Canopy

Note that the Academic version of Canopy comes with PySAL version 1.7. For this course we will be using PySAL 1.10. Upgrading in Canopy can be done as follows:

1. Install [Canopy][Canopy]
2. Run Canopy
3. From the menu select `Tools Canopy Terminal`
4. `pip install -U pysal`
5. `pip install -U folium`



#### Testing Your Installation

Once you have installed all the dependencies, you can check to confirm everything is ready to go.

For Anaconda:

1. Open a terminal (Mac or Linux) or Powershell (Windows)
2. `ipython notebook`
3. In the browser click `New Notebook`
3. In the first cell in the notebook enter  
   `import pysal`
   `pysal.version`
   Then `<Shift-Enter>` (i.e., hit the Shift then the Enter Key)
4. In the second cell in the notebook enter  
   `import folium`
   Then `<Shift-Enter>`
5. In the third cell enter
   `!which python`
   Then `<Shift-Enter>`
 
Your screen should look something like:
![Anaconda setup]({filename}/figures/anaconda.png)


For Enthought Canopy:

2. Run Canopy
3. From the menu select `Tools Canopy Terminal`
2. `ipython notebook`
3. In the browser click `New Notebook`
3. In the first cell in the notebook enter  
   `import pysal`
   `pysal.version`
   Then `<Shift-Enter>` (i.e., hit the Shift then the Enter Key)
4. In the second cell in the notebook enter  
   `import folium`
   Then `<Shift-Enter>`
5. In the third cell enter
   `!which python`
   Then `<Shift-Enter>`
 

Your screen should look something like:
![Enthought setup]({filename}/figures/enthought.png)

#### Issues

If you run into any problems, double check that you have installed both the upgraded version of PySAL and folium (see above). If problems persist, please contact me <srey@asu.edu>.


[PySAL]: http://pysal.org
[GeoDaSpace]: https://geodacenter.asu.edu/software/downloads/geodaspace
[Anaconda]: http://continuum.io/downloads.html
[Canopy]: https://www.enthought.com/store
[VirtualBox]: https://www.virtualbox.org/wiki/Downloads
[VirtualBox 4.3.12]: http://download.virtualbox.org/virtualbox/4.3.12/VirtualBox-4.3.12-93733-Win.exe
[Sergio Rey]: https://geoplan.asu.edu/people/sergio-j-rey
