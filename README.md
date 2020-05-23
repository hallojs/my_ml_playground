# My ML Playground
My machine learning playground.

## Requirements-Files and Virtual Enviroments
1. basic_data_science_requirements: A requirements file with the basic stuff needed for machine learning and data science. This file can be used as a basis for machine learning experiments and data science projects.

Build a virtual enviroment (VE) with the requiremnts from above:
1. Create a VE:
```bash
python3 -m venv <name of the VE>
```

2. Activate VE:
```bash
source <name of the VE>/bin/activate
```
To deactivate the VE just type (don't do it now, the VE must be activated for the following steps):
```bash
deactivate
```

3. Install requirements :
```bash
pip install -r <name of the requirements file>
```

4. Link VE to Jupyter Notebook
```bash
python -m ipykernel install --user --name=<name of the VE>
```
List all VEs available in jupyter notebook:
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
```

## Notebooks
1. autoencoder_anomaly_detection: Anomaly-detection in strings using an autoencoder. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/autoencoder_anomaly_detection.ipynb)
2. Evaluation of the differential private stochastic gradient descent in tensorflow-privacy on the mnist dataset. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hallojs/my_tf_playground/blob/master/mnist_dpsgd.ipynb)
