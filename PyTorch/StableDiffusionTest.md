# Install on Windows without GIT with conda

https://github.com/neonsecret/neonpeacasso  

https://huggingface.co/CompVis/stable-diffusion-v-1-4-original    

https://pytorch.org/get-started/locally/  

`pip3 install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cu116`

clone https://github.com/CompVis/taming-transformers  

pip install ./taming-transformers-master   

clone https://github.com/openai/CLIP

pip install ./CLIP-main  

clone https://github.com/neonsecret/stable-diffusion

pip install ./stable-diffusion-main  

comment CLIP & latent-diffusion in setup.py in neonpeacasso-master

clone https://github.com/neonsecret/neonpeacasso  

pip install ./neonpeacasso-master

fix error `AttributeError: module 'brotli' has no attribute 'error'`  

pip install brotli    

pip install taming-transformers-rom1504 (bug fix : https://github.com/CompVis/stable-diffusion/issues/84 )

neonpeacasso ui  --port=8080    

neonpeacasso ui  --host="0.0.0.0"  --port=8080  

give mode.ckpt path

test `portrait photo of a cat, 50mm portrait photography, hard rim lighting photography--beta`  

# Pytorch test  

```
import sys
import torch

print(f"PyTorch Version: {torch.__version__}\n")
print(f"Python {sys.version}\n")
print("GPU is", "available" if torch.cuda.is_available() else "NOT AVAILABLE")
```
