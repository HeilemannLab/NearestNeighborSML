# NearestNeighborSML
Investigation of nearest neighbor distributions of single molecule localizations (SML) in cells. The analysis is executed in a jupyter notebook (NearestNeighbor1234). The input files are hdf5 files that contain a column "com_x" for the x-localizations and a column "com_y" for the y-localizations of clusters, created in Picasso after the DBSCAN. The notebook requires four targets and two conditions. Since the names are input parameters, the notebooks can easily be applied to other measurements with different targets and measurement conditions.

### NearestNeighbor1234
This analysis compares four measured target (e.g. FGFR1/2/3/4) localization distributions between not active and active cells by using nearest neighbor distances:
- Calculate the nearest neighbor distances
- Calculate the percentage of nearest neighbor distances less or equal to a threshold
- Determine the nearest neighbor types

## Requirements
We recommend to run the notebooks in a virtual environment, for example via Anaconda/Miniconda with its powerful package manager.

### Set up the environment in conda & start the notebooks
1. open the anaconda prompt and create a new virtual environment: conda create --name NeighborDistributions python=3.7
2. activate the environment: conda activate NeighborDistributions
3. install the required packages (see below)
4. save the notebooks in a directory
5. navigate to the directory containing the notebooks in the anaconda prompt
6. run the notebooks with the command: jupyter notebook

### Install required packages
conda install -c anaconda h5py <br/>
conda install -c anaconda ipywidgets <br/>
conda install -c anaconda numpy <br/>
conda install -c anaconda pandas <br/>
conda install -c plotly plotly <br/>
conda install -c conda-forge tqdm <br/>

Install the following packages to get a clearer notebook:<br/>
conda install -c conda-forge jupyter_contrib_nbextensions<br/>
conda install -c conda-forge jupyter_nbextensions_configurator<br/>
Navigate to Nbextensions in the notebook process and check "Collapsible Headings"

Tested versions:
python: 3.7.6
h5py: 2.10.0
ipywidgets: 7.5.1
numpy: 1.18.1
pandas: 1.0.0
plotly: 4.5.0
tqdm: 4.42.0

## Literature
FGFR Methods Paper: M. S. Schröder, M.-L. I. E. Harwardt, J. V. Rahm, Y. Li, P. Freund, M. S. Dietz, M. Heilemann, *Imaging the fibroblast growth factor receptor network on the plasma membrane with DNA-assisted single-molecule super-resolution microscopy*, Methods in Extracellular Vesicles and Mimetics **2020**, DOI: https://doi.org/10.1016/j.ymeth.2020.05.004

Picasso: J. Schnitzbauer, M. T. Strauss, T. Schlichthaerle, F. Schueder, R. Jungmann,
*Super-Resolution Microscopy with DNA-PAINT*, Nature Protocols **2017**, *12*, 1198-1228; DOI: https://doi.org/10.1038/nprot.2017.024

## Web
For more information visit: https://www.uni-frankfurt.de/43272324/Welcome_to_the_homepage_of_the_Heilemann_Group
