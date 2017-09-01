# CIFAR 10 Dataset

This repo is basically aimed for easy transfer of data through the servers, but I kept it public as other people can probably benefit from it.

Just clone it, and use it! 
Here's the example code of how you could use it :

```python
import numpy as np

batch = np.load(file_path)
X, Y = batch[:, 1:], batch[:, 0]
```