# Tensorflow Developer Certificate Bootcamp

This repo contains the code from this [Udemy course](https://www.udemy.com/course/tensorflow-developer-certificate-machine-learning-zero-to-mastery/).

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

## Some useful working commands

### 1. Activating anaconda environment

conda activate \<environment\>

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

### 2. Starting Jupyter (Jupyter lab) in particular folder

jupyter notebook --notebook-dir="\<Path to desired working folder\>"

jupyter lab --notebook-dir="\<Path to desired working folder\>"

## Some notes on installation

#### 1. Install WSL2 according official instructions from Microsoft:

They can be found [here](https://learn.microsoft.com/en-us/windows/wsl/install)

#### 2. Install Miniconda using the following commands:

`
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -o Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
`

#### 3. Create conda environment:

`
conda create -n udemy-tensorflow-bootcamp
`

#### 4. Activate the environtment

`
conda activate udemy-tensorflow-bootcamp
`

#### 5. Activate the environtment

`
conda install python tensorflow tensorflow-gpu cudatoolkit cudnn scikit-learn pandas scipy matplotlib seaborn jupyter numpy==1.23.4
`

The **_numpy_** should be version **1.23.5** or lower in order to avoid 
***module 'numpy' has no attribute 'object'*** exceptions in **tensorflow**.

#### 6. Install numactl:

Tensorflow is complaining about **_numactl_**:

`
No NUMA support available on this system.
`

The solution to avoid this error:

`
sudo apt-get install numactl
`