# EvoLand Creat and Upload a STAC Collection Example Notebook

<img src="https://www.evo-land.eu/wp-content/themes/evoland/public/images/logo-evoland.png"
     alt="Evoland logo"
     />

This repository contains one Python Jupyter Notebooks showing an example of creating and uploading a STAC collection.


### Local Installation Instructions
To run the notebook locally execute the steps below (please note: the Anaconda Python environment has been tested on Linux Ubuntu 18.04, on Windows please use in step 3 the runtime optimized trimmed version `environment_windows.yml`):

1. Install Anaconda to manage virtual environments. You can follow the instructions [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).
2. Clone the repository and get into the repo folder:

3. A Terrascope account is required for the use of the stac-api. An account can be created [at](https://terrascope.be/en). Once the account is created, the credentials should be stored in a `.env` file in order to run the notebook (You can rename `.env.example` file or create a new `.env` file in the root folder).

4. Create a new conda environment with the following command:
```
        conda env create -f environment.yml
        conda env create -f environment_windows.yml (use this line on Windows)
```
5. Once the process is complete, you can activate the environment:
```
        conda activate stacbuilder-notebooks
```
6. Now you can start the Jupyter Notebook Server and use the notebooks, just typing:
```
        jupyter notebook
```
7. This should open up a new window in your default web browser, where you can select the notebook you prefer.

### Add new collections

The notebook relies heavily on [stac-catalog-builder](https://github.com/VitoTAP/stac-catalog-builder/tree/main) for the creation of STAC collections, and helper methods to work with the stac-api.

Documentation on how to configure a new dataset can be found at [link](https://github.com/VitoTAP/stac-catalog-builder/blob/main/docs/how-to-configure-new-dataset.md) and can be applied to this notebook as well.

1. Create a new folder under notebooks for the new dataset.
2. Create a `config-collection.json` file at the root of the new directory. A template file can be found at [config-collection.json](https://github.com/VitoTAP/stac-catalog-builder/blob/main/configs-datasets/config-template/config-collection.json), and fill the required fields in the file. 
3. Once set up, the collection can be created with CLI commands (see [docs](https://github.com/VitoTAP/stac-catalog-builder/blob/main/docs/how-to-run-stacbuilder.md)), or a [script](https://github.com/Evoland-Land-Monitoring-Evolution/stacbuilder-notebooks/blob/main/notebooks/SENTINEL2_L2A_NDVI_POTENTIAL/workflow.ipynb).