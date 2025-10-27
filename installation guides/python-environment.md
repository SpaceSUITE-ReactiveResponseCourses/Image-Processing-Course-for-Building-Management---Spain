Set up a working Python environment using conda.

Launch your Miniconda Prompt or Terminal.

Navigate to your UHI project folder.
Example:
cd path/to/uhi-project-folder

Create a conda environment in the project folder:
conda create --prefix ./uhi-env
conda activate ./uhi-env

Install required packages:
conda install geopandas localtileserver ipykernel jupyterlab earthengine-api -c conda-forge
conda install geemap -c conda-forge
pip install oeel
conda install nodejs=18.17.1

Install required npm packages inside the oeel directory:
cd ./uhi-env/Lib/site-packages/oeel
npm install zeromq@6.0.0-beta.6 unpromisefy
