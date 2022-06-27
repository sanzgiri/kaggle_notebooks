# kaggle_notebooks

## Running on Azure ML Workspace

* Create a new conda environment from a terminal in your compute instance using:
```
conda create -n py38 python=3.8
conda activate py38
conda install pip ipykernel
python -m ipykernel install --user --name python38 --display-name "Python 38"
```
* At this point, may need to restart compute environment. Go back to terminal and activate your environment again.
* Install fastai and any additional packages
```
conda install -c fastchan fastai
pip install git+https://github.com/fastai/fastkaggle
pip install -U timm
pip install -U jupyter ipywidgets
```