# Material for the ebook `Becoming a Spatial Data Scientist`

## Link here
### https://github.com/CartoDB/data-science-book

## Installation requirements

The notebooks in this repository use a ready-to-run Docker image containing Jupyter applications and interactive computing tools. To run the notebooks, please follow the instructions below.

### Clone the repository 

`$ git clone git@github.com:CartoDB/data-science-book.git`
`$ cd data-science-book`

### Download and install docker

Follow instructions here: https://docs.docker.com/install/

### Run the image

Open your terminal and run

```
$ docker run --user root -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -e GRANT_SUDO=yes -v "$PWD":/home/jovyan/workspace jupyter/datascience-notebook
```

A local address will be created. Copy and paste the address in your browser, this will launch Jupyter Lab.

**Note**: If you have another Jupyter server running, make sure it's on a different port than 8888. Otherwise change the port number above or close down the other notebook server.

### Install libraries and packages

Click New -> Terminal and go to the directory where you cloned the Github repository and run this script to install the required libraries

`$ bash notebooks_start.sh`

Note: the installation can take a while (10-15 min)

## Go to the `Chapters` folders and have fun :)

### Chapter 1 content:

- `Visualizing spatial data with CARTOframes.ipynb` - A Jupyter notebook for easily visualizing your data on a map using CARTOframes.

- `Computing measures of spatial dependence.ipynb` - A Jupyter notebook for exploring spatial dependence in your data and visualize the results using CARTOframes.

- `Discrete spatial models.ipynb` - A Jupyter notebook with examples of spatial models for discrete processes and visualize the results using CARTOframes.

- `Continous spatial models.ipynb` - A Jupyter notebook with examples of spatial models for continuous processes and visualize the results using CARTOframes.
