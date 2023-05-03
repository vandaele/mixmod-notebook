# mixmod-notebook

[![Binder](https://mybinder.org/badge_logo.svg)](https://notebooks.gesis.org/binder/v2/gh/vandaele/mixmod-notebook/master)

Run Rmixmod notebooks into the cloud using the Binder service by clicking the badge above.

If you need a persistent environment and/or more calculation power, follow the instructions in the next section.

## Run the notebooks locally with Docker

* Install Docker
* Clone this repository
  ```
  git clone https://github.com/vandaele/mixmod-notebook.git
  cd mixmod-notebook
  ```
* Launch a Docker container
  ```
  docker run --rm -p 8888:8888 -v ${PWD}:/home/jovyan vandaele/mixmod-notebook
  ```
  - `--rm` will automatically delete the container once stopped
  - `-p` redirects the Jupyter Notebook interface from the container to your local system
  - `-v` mounts the current directory (this repo) to the `home/jovyan` directory of the docker container
* Visit the link displayed in the console output to access the Jupyter interface
* Use Ctrl-C from the terminal, or the Quit button from the Jupyter interface to stop the container
