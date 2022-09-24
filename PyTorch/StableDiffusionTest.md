https://github.com/neonsecret/neonpeacasso  

https://huggingface.co/CompVis/stable-diffusion-v-1-4-original    

https://pytorch.org/get-started/locally/  

`pip3 install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cu116`

# Pytorch test  

```
import sys
import torch

print(f"PyTorch Version: {torch.__version__}\n")
print(f"Python {sys.version}\n")
print("GPU is", "available" if torch.cuda.is_available() else "NOT AVAILABLE")
```
