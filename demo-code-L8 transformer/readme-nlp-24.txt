To create your own envs:

conda create --name ann-transformer python=3.10
conda activate ann-transformer

For Mac Users:
pip install torch==1.11.0 torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cpu

Modify: requirements.txt file to:

--find-links https://download.pytorch.org/whl/torch_stable.html
pandas==1.3.5
# torch==1.11.0+cu113
torch==1.11.0
torchdata==0.3.0
torchtext==0.12
spacy==3.2
altair==4.1
jupytext==1.13
flake8
black
GPUtil
wandb

Then, you can do the following as suggested:

pip install -r requirements.txt

You may also need to install jupyter

conda install jupyter 

If it has an error like ModuleNotFoundError: No module named 'chardet',
please install the following:

conda install chardet

To download MT task dataset, go to:

git clone https://github.com/multi30k/dataset.git

