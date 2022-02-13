Ref : https://github.com/jeffheaton/t81_558_deep_learning/blob/master/install/pytorch-install-jul-2020.ipynb

Test Code: 

```
import sys

import torch
import pandas as pd
import sklearn as sk

print(f"PyTorch Version: {torch.__version__}")
print()
print(f"Python {sys.version}")
print(f"Pandas {pd.__version__}")
print(f"Scikit-Learn {sk.__version__}")
print("GPU is", "available" if torch.cuda.is_available() else "NOT AVAILABLE")
```

Expected Output:

```
PyTorch Version: 1.12.0.dev20220207

Python 3.9.7 (default, Sep 16 2021, 16:59:28) [MSC v.1916 64 bit (AMD64)]
Pandas 1.3.5
Scikit-Learn 1.0.2
GPU is available
```

