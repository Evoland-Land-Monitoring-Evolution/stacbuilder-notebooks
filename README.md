# openEO Platform User Oriented Example Notebooks

<img src="https://www.evo-land.eu/wp-content/themes/evoland/public/images/logo-evoland.png"
     alt="Evoland logo"
     />

This repository contains Python Jupyter Notebooks and R Notebooks, showing interactive examples of creating and uploading STAC collections.


### Local Installation Instructions
Alternatively, you can run them locally (please note: the Anaconda Python enviornment has been tested on Linux Ubuntu 18.04, on Windows please use in step 3 the runtime optimized trimmed version `environment_windows.yml`):

1. Install Anaconda to manage virtual environments. You can follow the instructions [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
2. Clone the repository and get into the repo folder:

3. Create a new conda environment with the following command:
```
        conda env create -f environment.yml
        conda env create -f environment_windows.yml (use this line on Windows)
```
4. Once the process is complete, you can activate the environment:
```
        conda activate stacbuilder-notebooks
```
5. Now you can start the Jupyter Notebook Server and use the notebooks, just typing:
```
        jupyter notebook
```
6. This should open up a new window in your default web browser, where you can select the notebook you prefer.