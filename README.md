



# Meeting monitoring dependencies


## 1. face detection
> - pip install mtcnn


## 2. tensorflow
> - pip install tensorflow==1.10
> - pip install tensorflow-gpu==1.10

> ### How to check if tensorflow is using GPU acceleration?

````
#Check if tensorflow is using GPU

import tensorflow as tf
	if tf.test.gpu_device_name():
		 print('Default GPU Device: {}'.format(tf.test.gpu_device_name()))
  else:
		 print("Please install GPU version of TF")
````
Expected result:
````
2020-01-22 15:13:08.867501: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1097]
Created TensorFlow device (/device:GPU:0 with 6304 MB memory) -> physical GPU (device: 0, name: GeForce GTX 1080, pci bus id: 0000:01:00.0, compute capability: 6.1)

Default GPU Device: /device:GPU:0
````


> If you have a compatible gpu and can use it, you will see the result. Otherwise, you will see an error with a long stacktrace.

## 3. Facial Landmarks Alignment

> ### - Pytorch Installation
- pip install torch==1.2.0

````
import torch as t
print(t.__version__)
````
> 1.2.0 should be printed out if pytorch was installed correctly.

> ### - Torchvision 0.4.0 Installation
- pip install torch torchvision==0.4.0
