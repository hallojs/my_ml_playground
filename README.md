# My ML Playground
My place to play around with machine learning and data science to learn and more importantly have fun :)

## Requirements-Files and Virtual Enviroments
1. basic_data_science_requirements: A requirements file with the basic stuff needed for machine learning and data science. This file can be used as a basis for machine learning experiments and data science projects.

Build a virtual enviroment (VE) with the requiremnts from above:
1. Create a VE:
```bash
python3 -m venv <name of the VE>
# or if you use pyenv-virtualenv:
pyenv virtualenv <python-version> <name of VE>
# show all VEs in pyenv:
pyenv virtualenvs
```

2. Activate VE:
```bash
source <name of the VE>/bin/activate
# and for pyenv-virtualenv:
pyenv activate <name of VE>
# or for convenience create a .python-version-file:
pyenv local <name of VE>
```
To deactivate the VE just type (don't do it now, the VE must be activated for the following steps):
```bash
deactivate
# or in pyenv:
pyenv deactivate
```

3. Install requirements :
```bash
pip install -r <name of the requirements file>
```

4. Link VE to Jupyter Notebook
```bash
python -m ipykernel install --user --name=<name of the VE>
```
List all VEs available in Jupyter Notebook:
```bash
jupyter kernelspec list
```
Delete Link from VE to Jupyter Notebook
```bash
jupyter kernelspec uninstall <name of the VE>
```

5. Delete VE from the system:
```bash
rm -r <path to VE>
# or in pyenv:
pyenv uninstall <name of VE>
```

## Notebooks
1. autoencoder_anomaly_detection: Anomaly-detection in strings using an autoencoder. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/autoencoder_anomaly_detection.ipynb)
2. mnist_dpsgd: Evaluation of the differential private stochastic gradient descent in tensorflow-privacy on the mnist dataset. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/mnist_dpsgd.ipynb)
3. input_generator_keras_model: In this notebook I experiment how to use generators as input for a keras model. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/input_generator_keras_model.ipynb)
4. keras_hyperparameter_tuning_tensorboard_hparams: In this notebook I use for the first time Tensorboard and HParams with a simple Keras model. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/keras_hyperparameter_tuning_tensorboard_hparams.ipynb)
The TensorBoard can be partially (without HParams plugin) found [here](https://tensorboard.dev/experiment/f6TagqsXRJW8pBkuoSyeQw/).
