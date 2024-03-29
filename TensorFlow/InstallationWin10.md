# TensorFlow Installation
## Windows 10 + CUDA + Anaconda
### TensorFlow 1.15
Ref 1: https://www.thehardwareguy.co.uk/install-tensorflow-gpu

Ref 2 : https://anaconda.org/anaconda/tensorflow-gpu/files

- (base) E:\Projects>conda create -n tf1 python=3.7
- (base) E:\Projects>conda activate tf1
- (tf1) E:\Projects>pip install ipykernel
- (tf1) E:\Projects>python -m ipykernel install --user --name tf1 --display-name "tf1"
- (tf1) E:\Projects>conda install tensorflow-gpu==1.15
- (tf1) E:\Projects>conda install jupyter
- (tf1) E:\Projects>jupyter notebook


### TensorFlow 2.3.1
Ref 1: https://www.thehardwareguy.co.uk/install-tensorflow-gpu

Ref 2: https://stackoverflow.com/questions/65273118/why-is-tensorflow-not-recognizing-my-gpu-after-conda-install/65319255#65319255 (Tensorflow v2.3.0 and does NOT install the conda cudnn or cudatoolkit packages)

- (base) E:\Projects>conda create -n tf2 python=3.7
- (base) E:\Projects>conda activate tf2
- (tf2) E:\Projects>pip install ipykernel
- (tf2) E:\Projects>python -m ipykernel install --user --name tf2 --display-name "tf2"
- (tf2) E:\Projects>conda install tensorflow-gpu==2.1
- (tf2) E:\Projects>pip install tensorflow-gpu==2.3.1
- (tf2) E:\Projects>conda install jupyter
- (tf2) E:\Projects>jupyter notebook

### TensorFlow 2.5
Ref 1: https://discuss.tensorflow.org/t/tensorflow-2-5-with-gpu-device-python-3-9-cuda-11-2-2-cudnn-8-1-1-conda-environment-windows-10/1385

- (base) E:\Projects>conda create -n tf2 python=3.9
- (base) E:\Projects>conda activate tf2
- (tf2) E:\Projects>conda install tensorflow-gpu
- (tf2) E:\Projects>conda install ipykernel
- (tf2) E:\Projects>python -m ipykernel install --user --name tf2 --display-name "Python 3.9 (Tensorflow 2.5)"
- (tf2) E:\Projects>conda install -c conda-forge notebook
- (tf2) E:\Projects>jupyter notebook

### Linux    

https://www.python-engineer.com/posts/setup-jupyter-notebook-in-conda-environment/   
`ipython kernel install --user --name=<any_name_for_kernel>` 

guide: https://www.hamvocke.com/blog/a-quick-and-easy-guide-to-tmux/    


tmux  
detach current session use CTRL+b, then d  

tmux ls   
tmux attach -t 0  

https://discourse.jupyter.org/t/how-to-run-a-notebook-using-command-line/3475/5   

`jupyter nbconvert --to notebook --execute mynotebook.ipynb`  


## Other useful libraries 

- conda install -c anaconda pillow 
- conda install -c numba numba 
- conda install -c conda-forge opencv 
- conda install -c conda-forge scikit-learn 
- conda install pandas
- pip install pydot
- pip install pydotplus
- conda install -c conda-forge matplotlib
- conda install -c plotly plotly
