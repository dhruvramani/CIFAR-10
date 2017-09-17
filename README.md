# CIFAR 10 Dataset

This repo is basically aimed for easy transfer of data through the servers, but I kept it public as other people can probably benefit from it.

Just clone it, and use it! 
Here's the example code of how you could use it :

```python
import pickle
import numpy as np

def load_data(file_name):
 with open(file_name, 'rb') as file:
  unpickler = pickle._Unpickler(file)
  unpickler.encoding = 'latin1'
  contents = unpickler.load()
  X, Y = contents['data'], contents['labels']
  return np.asarray(X), np.asarray(Y)
```
