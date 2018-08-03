### CUDA 및 cuDNN 설치
- 쿠다 툴킷만 설치하면 cuDNN은 아나콘다가 처리해주는 것 같음.  
  
  
### TensorFlow GPU 설치
- 사용자 환경을 새로 구성한다.  
- tfGPU로 구성하였다.  
- tfGPU로 사용자 환경을 바꾼다.(라이브러리가 하나도 없다.)  
- 텐서플로우 라이브러리(GPU용)를 설치한다.  
- 주피터 노트북을 설치한다. ...(이후는 알아서^^)  
- 주피터 노트북을 실행한 후 [gpucheck.ipynb](./gpucheck.ipynb)로 설치여부를 확인한다.  
***
- 사용자 환경을 새로 구성한다.  
~~~
(base) >conda create -n tfGPU
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
- tfGPU로 사용자 환경을 바꾼다.(라이브러리가 하나도 없다.)  
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
- 주피터 노트북을 설치한다.  
~~~
(tfGPU) D:\Data\[데이터]>conda install jupyter
Solving environment: done

## Package Plan ##

  environment location: D:\ProgramData\Anaconda3\envs\tfGPU

  added / updated specs:
    - jupyter


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    prometheus_client-0.3.1    |           py36_0          52 KB
    jedi-0.12.1                |           py36_0         225 KB
    pywinpty-0.5.4             |           py36_0          47 KB
    pyasn1-0.4.4               |           py36_0         101 KB
    automat-0.7.0              |           py36_0          70 KB
    pandoc-2.2.1               |       h1a437c5_0        20.4 MB
    appdirs-1.4.3              |           py36_0          16 KB
    zeromq-4.2.5               |       he025d50_1         9.5 MB
    pyasn1-modules-0.2.2       |           py36_0          86 KB
    incremental-17.5.0         |   py36he5b1da3_0          25 KB
    zope.interface-4.5.0       |   py36hfa6e2cd_0         203 KB
    ipython-6.5.0              |           py36_0         1.1 MB
    jupyter_core-4.4.0         |           py36_0          85 KB
    widgetsnbextension-3.3.1   |           py36_0         1.7 MB
    pandocfilters-1.4.2        |           py36_1          13 KB
    twisted-18.4.0             |   py36hfa6e2cd_0         5.0 MB
    parso-0.3.1                |           py36_0         115 KB
    nbconvert-5.3.1            |           py36_0         422 KB
    hyperlink-18.0.0           |           py36_0          62 KB
    ipywidgets-7.3.1           |           py36_0         148 KB
    entrypoints-0.2.3          |           py36_2           9 KB
    constantly-15.1.0          |           py36_0          13 KB
    qt-5.9.6                   |   vc14h62aca36_0        92.5 MB
    jinja2-2.10                |           py36_0         183 KB
    markupsafe-1.0             |   py36hfa6e2cd_1          27 KB
    zope-1.0                   |           py36_0           3 KB
    service_identity-17.0.0    |           py36_0          18 KB
    sqlite-3.24.0              |       h7602738_0         899 KB
    notebook-5.6.0             |           py36_0         7.3 MB
    pycparser-2.18             |           py36_1         169 KB
    tornado-5.0.2              |   py36hfa6e2cd_0         654 KB
    pyzmq-17.0.0               |   py36hfa6e2cd_3         398 KB
    idna-2.7                   |           py36_0         132 KB
    ------------------------------------------------------------
                                           Total:       141.6 MB

The following NEW packages will be INSTALLED:

    appdirs:                 1.4.3-py36_0
    asn1crypto:              0.24.0-py36_0
    attrs:                   18.1.0-py36_0
    automat:                 0.7.0-py36_0
    backcall:                0.1.0-py36_0
    ca-certificates:         2018.03.07-0
    cffi:                    1.11.5-py36h945400d_0
    colorama:                0.3.9-py36h029ae33_0
    constantly:              15.1.0-py36_0
    cryptography:            2.2.2-py36hfa6e2cd_0
    decorator:               4.3.0-py36_0
    entrypoints:             0.2.3-py36_2
    hyperlink:               18.0.0-py36_0
    icu:                     58.2-ha66f8fd_1
    idna:                    2.7-py36_0
    incremental:             17.5.0-py36he5b1da3_0
    ipykernel:               4.8.2-py36_0
    ipython:                 6.5.0-py36_0
    ipython_genutils:        0.2.0-py36h3c5d0ee_0
    ipywidgets:              7.3.1-py36_0
    jedi:                    0.12.1-py36_0
    jinja2:                  2.10-py36_0
    jpeg:                    9b-hb83a4c4_2
    jsonschema:              2.6.0-py36h7636477_0
    jupyter:                 1.0.0-py36_4
    jupyter_client:          5.2.3-py36_0
    jupyter_console:         5.2.0-py36h6d89b47_1
    jupyter_core:            4.4.0-py36_0
    libpng:                  1.6.34-h79bbb47_0
    libsodium:               1.0.16-h9d3ae62_0
    m2w64-gcc-libgfortran:   5.3.0-6
    m2w64-gcc-libs:          5.3.0-7
    m2w64-gcc-libs-core:     5.3.0-7
    m2w64-gmp:               6.1.0-2
    m2w64-libwinpthread-git: 5.0.0.4634.697f757-2
    markupsafe:              1.0-py36hfa6e2cd_1
    mistune:                 0.8.3-py36hfa6e2cd_1
    msys2-conda-epoch:       20160418-1
    nbconvert:               5.3.1-py36_0
    nbformat:                4.4.0-py36h3a5bc1b_0
    notebook:                5.6.0-py36_0
    openssl:                 1.0.2o-hfa6e2cd_1
    pandoc:                  2.2.1-h1a437c5_0
    pandocfilters:           1.4.2-py36_1
    parso:                   0.3.1-py36_0
    pickleshare:             0.7.4-py36h9de030f_0
    prometheus_client:       0.3.1-py36_0
    prompt_toolkit:          1.0.15-py36h60b8f86_0
    pyasn1:                  0.4.4-py36_0
    pyasn1-modules:          0.2.2-py36_0
    pycparser:               2.18-py36_1
    pygments:                2.2.0-py36hb010967_0
    pyopenssl:               18.0.0-py36_0
    pyqt:                    5.9.2-py36h1aa27d4_0
    pywin32:                 223-py36hfa6e2cd_1
    pywinpty:                0.5.4-py36_0
    pyzmq:                   17.0.0-py36hfa6e2cd_3
    qt:                      5.9.6-vc14h62aca36_0
    qtconsole:               4.3.1-py36h99a29a9_0
    send2trash:              1.5.0-py36_0
    service_identity:        17.0.0-py36_0
    simplegeneric:           0.8.1-py36_2
    sip:                     4.19.8-py36h6538335_0
    sqlite:                  3.24.0-h7602738_0
    terminado:               0.8.1-py36_1
    testpath:                0.3.1-py36h2698cfe_0
    tornado:                 5.0.2-py36hfa6e2cd_0
    traitlets:               4.3.2-py36h096827d_0
    twisted:                 18.4.0-py36hfa6e2cd_0
    wcwidth:                 0.1.7-py36h3d5aa90_0
    widgetsnbextension:      3.3.1-py36_0
    winpty:                  0.4.3-4
    zeromq:                  4.2.5-he025d50_1
    zope:                    1.0-py36_0
    zope.interface:          4.5.0-py36hfa6e2cd_0

Proceed ([y]/n)? y


Downloading and Extracting Packages
prometheus_client-0. |   52 KB | ################################################################################################## | 100%
jedi-0.12.1          |  225 KB | ################################################################################################## | 100%
pywinpty-0.5.4       |   47 KB | ################################################################################################## | 100%
pyasn1-0.4.4         |  101 KB | ################################################################################################## | 100%
automat-0.7.0        |   70 KB | ################################################################################################## | 100%
pandoc-2.2.1         | 20.4 MB | ################################################################################################## | 100%
appdirs-1.4.3        |   16 KB | ################################################################################################## | 100%
zeromq-4.2.5         |  9.5 MB | ################################################################################################## | 100%
pyasn1-modules-0.2.2 |   86 KB | ################################################################################################## | 100%
incremental-17.5.0   |   25 KB | ################################################################################################## | 100%
zope.interface-4.5.0 |  203 KB | ################################################################################################## | 100%
ipython-6.5.0        |  1.1 MB | ################################################################################################## | 100%
jupyter_core-4.4.0   |   85 KB | ################################################################################################## | 100%
widgetsnbextension-3 |  1.7 MB | ################################################################################################## | 100%
pandocfilters-1.4.2  |   13 KB | ################################################################################################## | 100%
twisted-18.4.0       |  5.0 MB | ################################################################################################## | 100%
parso-0.3.1          |  115 KB | ################################################################################################## | 100%
nbconvert-5.3.1      |  422 KB | ################################################################################################## | 100%
hyperlink-18.0.0     |   62 KB | ################################################################################################## | 100%
ipywidgets-7.3.1     |  148 KB | ################################################################################################## | 100%
entrypoints-0.2.3    |    9 KB | ################################################################################################## | 100%
constantly-15.1.0    |   13 KB | ################################################################################################## | 100%
qt-5.9.6             | 92.5 MB | ################################################################################################## | 100%
jinja2-2.10          |  183 KB | ################################################################################################## | 100%
markupsafe-1.0       |   27 KB | ################################################################################################## | 100%
zope-1.0             |    3 KB | ################################################################################################## | 100%
service_identity-17. |   18 KB | ################################################################################################## | 100%
sqlite-3.24.0        |  899 KB | ################################################################################################## | 100%
notebook-5.6.0       |  7.3 MB | ################################################################################################## | 100%
pycparser-2.18       |  169 KB | ################################################################################################## | 100%
tornado-5.0.2        |  654 KB | ################################################################################################## | 100%
pyzmq-17.0.0         |  398 KB | ################################################################################################## | 100%
idna-2.7             |  132 KB | ################################################################################################## | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: | DEBUG menuinst_win32:__init__(196): Menu: name: 'Anaconda${PY_VER} ${PLATFORM}', prefix: 'D:\ProgramData\Anaconda3\
envs\tfGPU', env_name: 'tfGPU', mode: 'system', used_mode: 'system'
DEBUG menuinst_win32:create(320): Shortcut cmd is D:\ProgramData\Anaconda3\python.exe, args are ['D:\\ProgramData\\Anaconda3\\cwp.py', 'D:\\
ProgramData\\Anaconda3\\envs\\tfGPU', 'D:\\ProgramData\\Anaconda3\\envs\\tfGPU\\python.exe', 'D:\\ProgramData\\Anaconda3\\envs\\tfGPU\\Scrip
ts\\jupyter-notebook-script.py', '%USERPROFILE%']
done
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
