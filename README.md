# python-learn
Learning Python from Scratch


## Local python environment setup

* Download & install miniforge3. Cut and paste the following command to a terminal window
  ```
  cd $HOME/Downloads
  curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
  ```

  Verify that you have downloaded the file, for example: `Miniforge3-Darwin-arm64.sh` by doing a `ls`.

* Run the installation script, follow the prompt:
  ```
  bash Miniforge3-$(uname)-$(uname -m).sh
  ```
* After the installation, you should have `conda` command installed, verify it by:
  ```
  conda env list
  ```
* Let's install a new python environment, we name it as "pylearn". We explicitly specify a python version we like to use, which is 3.14.

  ```
  conda create -n "pylearn" python=3.14
  ```
* Once an environment is created, we need to explicitly "activate" the environment. Note here we do it a bit differently, instead of running "conda activate pylearn" (which require a slightly different setup", we do it by:

  ```
  source activate pylearn
  ```
* Once environment is activated, we can install jupyter

  ```
  pip install jupyterlab
  pip install pandas
  ```
* Now, we have a local JupyterLab setup, which is the main learning environment, we can launch it by:

  ```
  jupyter lab
  ```

  you should expect a browswer window open - and you can create a new notebook from the sratch, or work on existing notebooks.

  


