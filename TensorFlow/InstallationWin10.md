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

## Other useful libraries 

- conda install -c anaconda pillow 
- conda install -c numba numba 
- conda install -c conda-forge opencv 