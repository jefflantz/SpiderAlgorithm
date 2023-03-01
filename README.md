# The Spider Algorithm

This directory contains an ipython notebook contianing Python code for the Spider Algorithm. Information on how it works and references are contained inside notebook.

This project was done by Jeffrey Lantz and Riley Guyett as part of their senior theses with Professor Hubbard in Spring 2023.

## Developer Notes
The python environment is managed via (mini)conda, which can be installed [here](https://docs.conda.io/projects/conda/en/stable/user-guide/install/index.html). The environment is managed in env.yaml, and should be automatically managed via git hooks. However, on initial install, one may need to run `conda env create -f env.yml`

Additionally, as working with Jupyter notebooks in version control can be difficult, we have included `nbstripout` in the conda environment. This may need to be manually initialized with `nbstripout --install --attributes .gitattributes`. This makes `git diff` show fewer non-code related changes, at the expense of not showing output data. I tried to include automatically generated outputs, but it wasn't working; for now, if we choose to include sample outputs in the repo, they will be added manually.

In order to run the Jupyter Notebook, simply call `jupyter lab` from the root directory of the repository, then select `spider-algorithm.ipynb` from the file explorer on the left. Jupyterlab supports a few nice features over jupyter notebook, accessible under `Settings > Advanced Settings Editor`. Here you can change the theme to dark under `Theme > Selected Theme`, and enable automatically formatting the code on saving the notebook under `Jupyterlab Code Formatter > Auto format config`.
