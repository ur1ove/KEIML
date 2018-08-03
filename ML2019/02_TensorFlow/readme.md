### CUDA 및 cuDNN 설치
  
  
### TensorFlow GPU 설치
- 사용자 환경을 새로 구성한다.  
- tfGPU로 구성하였다.  
>conda create -n tfGPU
~~~
Solving environment: done


==> WARNING: A newer version of conda exists. <==
  current version: 4.5.5
  latest version: 4.5.9

Please update conda by running

    $ conda update -n base -c defaults conda



## Package Plan ##

  environment location: D:\ProgramData\Anaconda3\envs\tfGPU


Proceed ([y]/n)? y

Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use:
# > activate tfGPU
#
# To deactivate an active environment, use:
# > deactivate
#
# * for power-users using bash, you must source
#
~~~
~~~
(base) >activate tfGPU

(tfGPU) >conda list
# packages in environment at D:\ProgramData\Anaconda3\envs\tfGPU:
#
# Name                    Version                   Build  Channel
~~~
- 텐서플로우 라이브러리(GPU용)를 설치한다.  
~~~
(tfGPU) >conda install tensorflow-gpu
Solving environment: done

## Package Plan ##

  environment location: D:\ProgramData\Anaconda3\envs\tfGPU

  added / updated specs:
    - tensorflow-gpu


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    absl-py-0.3.0              |           py36_0         137 KB
    mkl_fft-1.0.4              |   py36h1e22a9b_1         120 KB
    tensorboard-1.8.0          |   py36he025d50_0         3.1 MB
    tensorflow-gpu-base-1.8.0  |   py36h376609f_0        75.4 MB
    mkl_random-1.0.1           |   py36h77b88f5_1         268 KB
    html5lib-0.9999999         |           py36_0         178 KB
    numpy-base-1.15.0          |   py36h4a99626_0         3.9 MB
    cudnn-7.1.4                |        cuda9.0_0       192.3 MB
    bleach-1.5.0               |           py36_0          22 KB
    grpcio-1.12.1              |   py36h1a1b453_0         1.4 MB
    astor-0.7.1                |           py36_0          44 KB
    termcolor-1.1.0            |           py36_1           8 KB
    numpy-1.15.0               |   py36h9fa60d3_0          36 KB
    mkl-2018.0.3               |                1       178.1 MB
    libprotobuf-3.5.2          |       he0781b1_0         2.0 MB
    markdown-2.6.11            |           py36_0         122 KB
    setuptools-39.2.0          |           py36_0         571 KB
    six-1.11.0                 |           py36_1          21 KB
    tensorflow-gpu-1.8.0       |       h21ff451_0           4 KB
    cudatoolkit-9.0            |                1       339.8 MB
    intel-openmp-2018.0.3      |                0         1.7 MB
    python-3.6.6               |       hea74fb7_0        21.6 MB
    protobuf-3.5.2             |   py36h6538335_0         512 KB
    gast-0.2.0                 |           py36_0          15 KB
    ------------------------------------------------------------
                                           Total:       821.1 MB

The following NEW packages will be INSTALLED:

    absl-py:             0.3.0-py36_0
    astor:               0.7.1-py36_0
    blas:                1.0-mkl
    bleach:              1.5.0-py36_0
    certifi:             2018.4.16-py36_0
    cudatoolkit:         9.0-1
    cudnn:               7.1.4-cuda9.0_0
    gast:                0.2.0-py36_0
    grpcio:              1.12.1-py36h1a1b453_0
    html5lib:            0.9999999-py36_0
    icc_rt:              2017.0.4-h97af966_0
    intel-openmp:        2018.0.3-0
    libprotobuf:         3.5.2-he0781b1_0
    markdown:            2.6.11-py36_0
    mkl:                 2018.0.3-1
    mkl_fft:             1.0.4-py36h1e22a9b_1
    mkl_random:          1.0.1-py36h77b88f5_1
    numpy:               1.15.0-py36h9fa60d3_0
    numpy-base:          1.15.0-py36h4a99626_0
    pip:                 10.0.1-py36_0
    protobuf:            3.5.2-py36h6538335_0
    python:              3.6.6-hea74fb7_0
    setuptools:          39.2.0-py36_0
    six:                 1.11.0-py36_1
    tensorboard:         1.8.0-py36he025d50_0
    tensorflow-gpu:      1.8.0-h21ff451_0
    tensorflow-gpu-base: 1.8.0-py36h376609f_0
    termcolor:           1.1.0-py36_1
    vc:                  14.1-h0510ff6_3
    vs2015_runtime:      15.5.2-3
    werkzeug:            0.14.1-py36_0
    wheel:               0.31.1-py36_0
    wincertstore:        0.2-py36h7fe50ca_0
    zlib:                1.2.11-h8395fce_2

Proceed ([y]/n)? y

Downloading and Extracting Packages
absl-py-0.3.0        |  137 KB | ################################################################################################## | 100%
mkl_fft-1.0.4        |  120 KB | ################################################################################################## | 100%
tensorboard-1.8.0    |  3.1 MB | ################################################################################################## | 100%
tensorflow-gpu-base- | 75.4 MB | ################################################################################################## | 100%
mkl_random-1.0.1     |  268 KB | ################################################################################################## | 100%
html5lib-0.9999999   |  178 KB | ################################################################################################## | 100%
numpy-base-1.15.0    |  3.9 MB | ################################################################################################## | 100%
cudnn-7.1.4          | 192.3 MB | ################################################################################################# | 100%
bleach-1.5.0         |   22 KB | ################################################################################################## | 100%
grpcio-1.12.1        |  1.4 MB | ################################################################################################## | 100%
astor-0.7.1          |   44 KB | ################################################################################################## | 100%
termcolor-1.1.0      |    8 KB | ################################################################################################## | 100%
numpy-1.15.0         |   36 KB | ################################################################################################## | 100%
mkl-2018.0.3         | 178.1 MB | ################################################################################################# | 100%
libprotobuf-3.5.2    |  2.0 MB | ################################################################################################## | 100%
markdown-2.6.11      |  122 KB | ################################################################################################## | 100%
setuptools-39.2.0    |  571 KB | ################################################################################################## | 100%
six-1.11.0           |   21 KB | ################################################################################################## | 100%
tensorflow-gpu-1.8.0 |    4 KB | ################################################################################################## | 100%
cudatoolkit-9.0      | 339.8 MB | ################################################################################################# | 100%
intel-openmp-2018.0. |  1.7 MB | ################################################################################################## | 100%
python-3.6.6         | 21.6 MB | ################################################################################################## | 100%
protobuf-3.5.2       |  512 KB | ################################################################################################## | 100%
gast-0.2.0           |   15 KB | ################################################################################################## | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
~~~
- 판다스 라이브러리도 설치한다.
~~~
(tfGPU) >conda install pandas
Solving environment: done

## Package Plan ##

  environment location: D:\ProgramData\Anaconda3\envs\tfGPU

  added / updated specs:
    - pandas


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    pytz-2018.5                |           py36_0         232 KB
    pandas-0.23.3              |   py36h830ac7b_0         8.6 MB
    ------------------------------------------------------------
                                           Total:         8.9 MB

The following NEW packages will be INSTALLED:

    pandas:          0.23.3-py36h830ac7b_0
    python-dateutil: 2.7.3-py36_0
    pytz:            2018.5-py36_0

Proceed ([y]/n)? y


Downloading and Extracting Packages
pytz-2018.5          |  232 KB | ################################################################################################## | 100%
pandas-0.23.3        |  8.6 MB | ################################################################################################## | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
~~~
