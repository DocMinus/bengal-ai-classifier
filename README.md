# bengal-ai-classifier

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DocMinus/bengal-ai-classifier/main?filepath=bengal_vs_cats_app.ipynb)

*Click on the icon for running this app directly! The startup of the "mybinder.org" app can take some time, so be patient!*

This is a simple proof of concept Jupyter to web-app, using a FastAI (Pytorch based) deep learning classifier of cat-pictures. It focuses on Bengal cats.

The classification is simply<br> 
*bengal / other / cartoon*

More edit:<br>
- *export.pkl* is the model file.
- *tmp.jpg* is cat picture to test if one doesn't have one handy.
- update: new model file. slightly better bengal detection
- update: use of GIT LFS for large files due to pkl > 25MB
- update: type on binder link corrected, requirements corrected.
- update: model creation file added.

## How to run

This is mainly intended to be run as a binder app by clicking on above "launchBinder" icon.<br>

For the more advnaced/interested:<br> 
You could also download the repo and run the Jupyter Notebook in a Conda environment (see requirements.txt, or the .yml file mentioned below).<br>
Yet another option would be manually by going to [MyBinder.org](https://mybinder.org) and fill out the form:<br>

Enter the following:<br>
Github: https://github.com/DocMinus/bengal-ai-classifier <br>
tags: main <br>
path (url, not file): bengal_vs_cats_app.ipynb <br>
As mentioned, the startup of the "mybinder.org" app can take some time, so be patient 

<br>
Also included: Jupyter notebook with the acutal model-creation (bengal_vs_cats_model_creation.ipynb), for completness sake. Not linked / guaranteed to work with Binder.

## Issues
None that I am aware of.

## Kudos
Based on [fast.ai](https://www.fast.ai/).

## Note to self
*requirements.yml* file that works (missing Voila though, should be added as well):

name: fastai
channels:
  - pytorch
  - defaults
dependencies:
  - pip
  - pytorch[version='>=1.6']
  - torchvision
  - python[version='>=3.6']
  - pip:
    - fastai>2.1

alternatively, use the current *requirements.txt* , this also includes Voila to allow for direct running of the code.
