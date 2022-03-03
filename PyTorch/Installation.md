# PyTorch Nightly Installation
## Windows 10 + CUDA + Anaconda

Ref: https://pytorch.org/get-started/locally/

```
conda create -n pyt python=3.9
conda activate pyt
conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch-nightly


conda install ipykernel
python -m ipykernel install --user --name pyt --display-name "Python 3.9 (PyTorch)"
conda install -c conda-forge notebook
jupyter notebook


conda install -c anaconda pillow
conda install -c numba numba
conda install -c conda-forge opencv
conda install -c conda-forge scikit-learn
conda install pandas
conda install -c conda-forge matplotlib
conda install -c plotly plotly
```


VSCode: https://github.com/numpy/numpy/issues/15183#issuecomment-603575874
