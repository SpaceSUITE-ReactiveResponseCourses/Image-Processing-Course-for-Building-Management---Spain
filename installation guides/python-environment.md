Set up a working python environment using conda. 

Launch your miniconda window and navigate to your uhi project folder.

Create a conda environment in your project folder

- conda create --prefix .\uhi-env
- conda activate .\uhi-env

Install packages
- conda install geopandas localtileserver ipykernel jupyterlab earthengine-api -c conda-forge
- conda install geemap -c conda-forge
- pip install oeel
- conda install nodejs=18.17.1


Install npm packages inside the oeel folder
- cd .\uhi-env\Lib\site-packages\oeel
- npm install zeromq@6.0.0-beta.6 unpromisefy
