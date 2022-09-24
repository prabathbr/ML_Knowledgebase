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

comment CLIP & latent-diffusion in swtup.py in neonpeacasso-master

clone https://github.com/neonsecret/neonpeacasso  

pip install ./neonpeacasso-master

# Pytorch test  

```
import sys
import torch

print(f"PyTorch Version: {torch.__version__}\n")
print(f"Python {sys.version}\n")
print("GPU is", "available" if torch.cuda.is_available() else "NOT AVAILABLE")
```
