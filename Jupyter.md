'''
nohup jupyter-lab --ip 0.0.0.0 --no-browser --allow-root &
'''
### Attach conda env to jupyter
'''
conda install -c anaconda ipykernel
python -m ipykernel install --user --name=firstEnv
'''

### installing jupyter server
'''
conda create -n influencer python==3.9,
pip install jupyterlab
jupyter notebook --generate-config 
or
jupyter-lab --generate-config

jupyter notebook password
jupyter-lab password


'''