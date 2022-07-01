# T-DEV-810-group16 Applications of Deep Neural Networks
 
# Software Installation
This class is technically oriented.  A successful student needs to be able to compile and execute Python code that makes use of TensorFlow for deep learning. There are two options for you to accomplish this:

* Install Python, TensorFlow and some IDE (Jupyter, TensorFlow, and others)

## Installing Python and TensorFlow

It is possible to install and run Python/TensorFlow entirely from your computer.  Google provides TensorFlow for Windows, Mac, and Linux.  Previously, TensorFlow did not support Windows.  However, as of December 2016, TensorFlow supports Windows for both CPU and GPU operation.

The first step is to install Python 3.9.  This is the latest version of Python 3.  I recommend using the Miniconda (Anaconda) release of Python, as it already includes many of the data science related packages that are needed by this class.  Anaconda directly supports Windows, Mac, and Linux.  Miniconda is the minimal set of features from the extensive Anaconda Python distribution.  Download Miniconda from the following URL:

* [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

# Python 3.9

*Note: I will remove this section once all needed libraries add support for Python 3.9.

**execute the following commands:** 

```
conda create -y --name tensorflow python=3.9
```

To enter this environment, you must use the following command (**for Windows**), this command must be done every time you open a new Anaconda/Miniconda terminal window:

```
activate tensorflow
```


For **Mac**, do this:

```
source activate tensorflow
```

# Installing Jupyter

it is easy to install Jupyter notebooks with the following command:

```
conda install -y jupyter
```

Once Jupyter is installed, it is started with the following command:

```
jupyter notebook
```

The following packages are needed :

```
conda install -y scipy
pip install --exists-action i --upgrade sklearn
pip install --exists-action i --upgrade pandas
pip install --exists-action i --upgrade pandas-datareader
pip install --exists-action i --upgrade matplotlib
pip install --exists-action i --upgrade pillow
pip install --exists-action i --upgrade tqdm
pip install --exists-action i --upgrade requests
pip install --exists-action i --upgrade h5py
pip install --exists-action i --upgrade pyyaml
pip install --exists-action i --upgrade tensorflow_hub
pip install --exists-action i --upgrade bayesian-optimization
pip install --exists-action i --upgrade spacy
pip install --exists-action i --upgrade gensim
pip install --exists-action i --upgrade flask
pip install --exists-action i --upgrade boto3
pip install --exists-action i --upgrade gym
pip install --exists-action i --upgrade opencv-python
pip install --exists-action i --upgrade tensorflow
pip install --exists-action i --upgrade keras
conda update -y --all
```

You should also link your new **tensorflow** environment to Jupyter so that you can choose it as a Kernal.  Always make sure to run your Jupyter notebooks from your 3.9 kernel.

```
python -m ipykernel install --user --name tensorflow --display-name "Python 3.6 (tensorflow)"
```
```
# What version of Python do you have?
import sys

import tensorflow.keras
import pandas as pd
import sklearn as sk
import tensorflow as tf

print(f"Tensor Flow Version: {tf.__version__}")
print(f"Keras Version: {tensorflow.keras.__version__}")
print()
print(f"Python {sys.version}")
print(f"Pandas {pd.__version__}")
print(f"Scikit-Learn {sk.__version__}")
print("GPU is", "available" if tf.test.is_gpu_available() else "NOT AVAILABLE")
```
