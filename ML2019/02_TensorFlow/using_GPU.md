- GPU용 텐서플로우는 텐서플로우를 설치하고 설치해야 함.
~~~
root@DataLX01:~# pip uninstall tensorflow-gpu
Uninstalling tensorflow-gpu-1.11.0:
  Would remove:
    /usr/local/bin/freeze_graph
    /usr/local/bin/saved_model_cli
    /usr/local/bin/tensorboard
    /usr/local/bin/tflite_convert
    /usr/local/bin/toco
    /usr/local/bin/toco_from_protos
    /usr/local/lib/python3.6/dist-packages/tensorflow/*
    /usr/local/lib/python3.6/dist-packages/tensorflow_gpu-1.11.0.dist-info/*
Proceed (y/n)? y
  Successfully uninstalled tensorflow-gpu-1.11.0
root@DataLX01:~# pip uninstall tensorflow
Uninstalling tensorflow-1.10.1:
  Would remove:
    /usr/local/lib/python3.6/dist-packages/tensorflow-1.10.1.dist-info/*
Proceed (y/n)? y
  Successfully uninstalled tensorflow-1.10.1
root@DataLX01:~# 
~~~
~~~
root@DataLX01:~# pip install tensorflow
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Collecting tensorflow
  Downloading http://mirror.kakao.com/pypi/packages/ce/d5/38cd4543401708e64c9ee6afa664b936860f4630dd93a49ab863f9998cd2/tensorflow-1.11.0-cp36-cp36m-manylinux1_x86_64.whl (63.0MB)
    100% |████████████████████████████████| 63.0MB 12.0MB/s 
Requirement already satisfied: wheel>=0.26 in /usr/lib/python3/dist-packages (from tensorflow) (0.29.0)
Requirement already satisfied: numpy>=1.13.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.14.3)
Requirement already satisfied: keras-applications>=1.0.5 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.0.6)
Requirement already satisfied: astor>=0.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (0.6.2)
Requirement already satisfied: six>=1.10.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.11.0)
Requirement already satisfied: protobuf>=3.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (3.6.1)
Requirement already satisfied: tensorboard<1.12.0,>=1.11.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.11.0)
Requirement already satisfied: termcolor>=1.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.1.0)
Requirement already satisfied: grpcio>=1.8.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.10.0)
Requirement already satisfied: setuptools<=39.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (39.1.0)
Requirement already satisfied: absl-py>=0.1.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (0.1.12)
Requirement already satisfied: keras-preprocessing>=1.0.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (1.0.5)
Requirement already satisfied: gast>=0.2.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow) (0.2.0)
Requirement already satisfied: h5py in /usr/local/lib/python3.6/dist-packages (from keras-applications>=1.0.5->tensorflow) (2.7.1)
Requirement already satisfied: werkzeug>=0.11.10 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.12.0,>=1.11.0->tensorflow) (0.14.1)
Requirement already satisfied: markdown>=2.6.8 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.12.0,>=1.11.0->tensorflow) (2.6.11)
Installing collected packages: tensorflow
Successfully installed tensorflow-1.11.0
root@DataLX01:~# pip install tensorflow-gpu
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Collecting tensorflow-gpu
  Downloading http://mirror.kakao.com/pypi/packages/25/52/01438b81806765936eee690709edc2a975472c4e9d8d465a01840869c691/tensorflow_gpu-1.11.0-cp36-cp36m-manylinux1_x86_64.whl (258.8MB)
    100% |████████████████████████████████| 258.8MB 12.6MB/s 
Requirement already satisfied: protobuf>=3.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (3.6.1)
Requirement already satisfied: six>=1.10.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.11.0)
Requirement already satisfied: setuptools<=39.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (39.1.0)
Requirement already satisfied: wheel>=0.26 in /usr/lib/python3/dist-packages (from tensorflow-gpu) (0.29.0)
Requirement already satisfied: absl-py>=0.1.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.1.12)
Requirement already satisfied: keras-applications>=1.0.5 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.0.6)
Requirement already satisfied: keras-preprocessing>=1.0.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.0.5)
Requirement already satisfied: numpy>=1.13.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.14.3)
Requirement already satisfied: termcolor>=1.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.1.0)
Requirement already satisfied: gast>=0.2.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.2.0)
Requirement already satisfied: tensorboard<1.12.0,>=1.11.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.11.0)
Requirement already satisfied: astor>=0.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.6.2)
Requirement already satisfied: grpcio>=1.8.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.10.0)
Requirement already satisfied: h5py in /usr/local/lib/python3.6/dist-packages (from keras-applications>=1.0.5->tensorflow-gpu) (2.7.1)
Requirement already satisfied: markdown>=2.6.8 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.12.0,>=1.11.0->tensorflow-gpu) (2.6.11)
Requirement already satisfied: werkzeug>=0.11.10 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.12.0,>=1.11.0->tensorflow-gpu) (0.14.1)
Installing collected packages: tensorflow-gpu
Successfully installed tensorflow-gpu-1.11.0
root@DataLX01:~# 
~~~
- 파이썬에서 아래 코드 실행 시 
~~~
from tensorflow.python.client import device_lib
print(device_lib.list_local_devices())
~~~
~~~
[name: "/device:CPU:0"
device_type: "CPU"
memory_limit: 268435456
locality {
}
incarnation: 7318764170464801508
, name: "/device:GPU:0"
device_type: "GPU"
memory_limit: 172228608
locality {
  bus_id: 2
  numa_node: 1
  links {
  }
}
incarnation: 14673047010294188329
physical_device_desc: "device: 0, name: Tesla M4, pci bus id: 0000:88:00.0, compute capability: 5.2"
]
~~~
