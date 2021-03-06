# Workshop on Domain-Specific Languages for Performance-Portable Weather and Climate Models

Material of the workshop held together with NOAA in 2020

## Setup on Orion

1. Log on to orion with `ssh <user>@orion-login.hpc.msstate.edu`
2. Check out the repository for the workshop `git clone https://github.com/VulcanClimateModeling/dsl_workshop.git workshop`
3. Add the line `if [ -f ~/workshop/setup/jupyter_env ] ; then source ~/workshop/setup/jupyter_env ; fi` to the file `.bashrc` just before the line `if [ -z "$PS1" ]; then return; fi`
4. Make sure current `.bashrc` is active by typing `exec bash`
5. Check `gcc --version` is 8.3.0
6. Load a current version of Python with `module load python/3.7.5`
7. Install GT4Py and setup Python virtual environment as Jupyter kernel with `source workshop/setup/setup_venv`

Note: At the end of the workshop you will want to remove the modification to your `~/.bashrc` again if you continue to use the Orion system.

## Connect to Jupyter on Orion

1. Point your browser to https://orion-ood.hpc.msstate.edu/
2. Click "Jupyter Notebook" under the "Interactive Apps" dropdown menu
3. Configure your session (Account Name = "gfdlhires", Partition Name = "development") and launch you session.
4. Once the session has started, click "Connect to Jupyter"
5. The material for the workshop is under `workshop/notebooks`
