# bengal-ai-classifier

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DocMinus/bengal-ai-classifier/main?urlpath=%2Fvoila%2Frender%2F%20bengal_vs_cats_app.ipynb)

This is a simple proof of concept Jupyter to web-app, using a FastAI (Pytorch based) deep learning classifier of cat-pictures. It focuses on Bengal cats.

The classification is simply<br> 
*bengal / other / cartoon*

**!The startup of the "mybinder.org" app can take some time, so be patient.!**

Note to self:<br>
*requirements.txt* is necessaryfor mybinder to work. Also requires the tag "main" to work properly.

More edit:<br>
- *export.pkl* is the model file.
- *tmp.jpg* is cat picture to test if one doesn't have one handy.
- update: new model file. slightly better bengal detection
- update: use of GIT LFS for large files due to pkl > 25MB

## How to run

You can either download the repo and run the Jupyter Notebook in your environment direclty (though I suggest you use a fresh Anaconda environmnet) or you can simply click on the "launch-binder" icon.
This can also be done manually, by going to [MyBinder.org]{https://mybinder.org} and fill out the form:

Enter the following:
Github: https://github.com/DocMinus/bengal-ai-classifier
tags: main
path (url, not file): /voila/render/bengal_vs_cats_app.ipynb <br>
As mentioned, the startup of the "mybinder.org" app can take some time, so be patient

## Issues
For some reason, mybinder throws an error and this doesn't work anymore. I am not sure if this is due to the large file system or something different.<br>
Meaning, if someone wants to test this, you will have to do the local Jupyter version.

## Kudos
Based on [fast.ai]{https://www.fast.ai/}.
