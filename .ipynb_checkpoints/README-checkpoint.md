# adverse_intent_detector

Spot and detect adverse comments using deep learning and python.

---

## Kaggle Dataset
### Dataset Link
https://www.kaggle.com/datasets/julian3833/jigsaw-toxic-comment-classification-challenge

### cudnn Installation Issue
Can't you install cudnn=8.6?   
Currently, conda only provides the package of cudnn=8.6 for Linux/macOS. Windows users don't have...

### Workaround
Install tensorflow without designating a version.   
It will automatically pull the corresponding cudatoolkit and cudnn, and you don't need to install them manually.     

### Caution
TensorFlow 2.10 was the last TensorFlow release that supported GPU on native - Windows.   
Starting with TensorFlow 2.11, you will need to install TensorFlow in WSL2, or install tensorflow or tensorflow - cpu and,   
optionally, try the TensorFlow - DirectML - Plugin.

### Gradio Introduction
Gradio is an open - source Python package that allows you to quickly build a demo or web application  
for your machine learning model, API, or any arbitrary Python function.

### Gradio Docs
https://www.gradio.app/guides/quickstart

---

## h5py Import Error

### Problem
The model can be trained normally, but it cannot be saved or loaded properly for the locally trained model.

If you use the local Jupyter Notebook, the following errors may occur (even if `h5py` is installed):
1. `ImportError: DLL load failed while importing defs: The specified program cannot be found.`
2. `ImportError: Filepath looks like a hdf5 file but h5py is not available. filepath=detector_model.h5`

### Solution
Install Jupyter Notebook or Jupyter Lab in the virtual environment:
```bash
pip install notebook
python -m notebook
```

### Reason Analysis
The previous project has made the local environment unclean.