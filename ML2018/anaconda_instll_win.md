- 연구환경 만들기 : Anaconda Prompt를 관리자 권한으로 실행합니다.  
  
~~~
(base) C:\Windows\system32>conda create -n tutorial python=3.6 numpy scipy matplotlib spyder pandas seaborn scikit-learn h5py
~~~
~~~
    zlib:                     1.2.11-h8395fce_2

Proceed ([y]/n)? y


Downloading and Extracting Packages
mccabe-0.6.1         |   13 KB | ###################################### | 100%
tornado-5.1          |  669 KB | ###################################### | 100%
spyder-kernels-0.2.6 |   70 KB | ###################################### | 100%
kiwisolver-1.0.1     |   61 KB | ###################################### | 100%
python-3.6.6         | 21.6 MB | ###################################### | 100%
nbconvert-5.3.1      |  422 KB | ###################################### | 100%
jupyter_core-4.4.0   |   85 KB | ###################################### | 100%
scipy-1.1.0          | 13.6 MB | ###################################### | 100%
sphinxcontrib-websup |   36 KB | ###################################### | 100%
pandoc-2.2.3.2       | 21.0 MB | ###################################### | 100%
ipykernel-4.9.0      |  147 KB | ###################################### | 100%
qtconsole-4.4.1      |  174 KB | ###################################### | 100%
pyzmq-17.1.2         |  401 KB | ###################################### | 100%
spyder-3.3.1         |  2.6 MB | ###################################### | 100%
psutil-5.4.7         |  323 KB | ###################################### | 100%
pycparser-2.18       |  169 KB | ###################################### | 100%
openssl-1.0.2p       |  5.4 MB | ###################################### | 100%
sphinxcontrib-1.0    |    3 KB | ###################################### | 100%
sip-4.19.12          |  283 KB | ###################################### | 100%
keyring-13.2.1       |   64 KB | ###################################### | 100%
urllib3-1.23         |  152 KB | ###################################### | 100%
seaborn-0.9.0        |  379 KB | ###################################### | 100%
mkl_fft-1.0.4        |  120 KB | ###################################### | 100%
freetype-2.9.1       |  470 KB | ###################################### | 100%
lazy-object-proxy-1. |   31 KB | ###################################### | 100%
pyflakes-2.0.0       |  106 KB | ###################################### | 100%
qtpy-1.5.0           |   53 KB | ###################################### | 100%
zeromq-4.2.5         |  9.5 MB | ###################################### | 100%
pandas-0.23.4        |  8.6 MB | ###################################### | 100%
intel-openmp-2018.0. |  1.7 MB | ###################################### | 100%
pylint-2.1.1         |  864 KB | ###################################### | 100%
numpy-base-1.15.1    |  3.9 MB | ###################################### | 100%
idna-2.7             |  132 KB | ###################################### | 100%
win_inet_pton-1.0.1  |    6 KB | ###################################### | 100%
h5py-2.8.0           |  835 KB | ###################################### | 100%
markupsafe-1.0       |   27 KB | ###################################### | 100%
certifi-2018.8.24    |  140 KB | ###################################### | 100%
pyparsing-2.2.0      |   96 KB | ###################################### | 100%
typed-ast-1.1.0      |  140 KB | ###################################### | 100%
astroid-2.0.4        |  250 KB | ###################################### | 100%
chardet-3.0.4        |  210 KB | ###################################### | 100%
jinja2-2.10          |  183 KB | ###################################### | 100%
mkl_random-1.0.1     |  268 KB | ###################################### | 100%
mkl-2018.0.3         | 178.1 MB | ##################################### | 100%
sphinx-1.7.8         |  1.6 MB | ###################################### | 100%
cffi-1.11.5          |  213 KB | ###################################### | 100%
numpy-1.15.1         |   37 KB | ###################################### | 100%
imagesize-1.1.0      |   10 KB | ###################################### | 100%
qt-5.9.6             | 92.5 MB | ###################################### | 100%
jedi-0.12.1          |  225 KB | ###################################### | 100%
cryptography-2.3.1   |  509 KB | ###################################### | 100%
parso-0.3.1          |  115 KB | ###################################### | 100%
sqlite-3.24.0        |  899 KB | ###################################### | 100%
cloudpickle-0.5.5    |   27 KB | ###################################### | 100%
entrypoints-0.2.3    |    9 KB | ###################################### | 100%
pytz-2018.5          |  232 KB | ###################################### | 100%
pyqt-5.9.2           |  4.6 MB | ###################################### | 100%
bleach-2.1.4         |   33 KB | ###################################### | 100%
webencodings-0.5.1   |   19 KB | ###################################### | 100%
requests-2.19.1      |   96 KB | ###################################### | 100%
setuptools-40.2.0    |  575 KB | ###################################### | 100%
ipython-6.5.0        |  1.1 MB | ###################################### | 100%
six-1.11.0           |   21 KB | ###################################### | 100%
wrapt-1.10.11        |   44 KB | ###################################### | 100%
matplotlib-2.2.3     |  6.5 MB | ###################################### | 100%
pandocfilters-1.4.2  |   13 KB | ###################################### | 100%
rope-0.11.0          |  282 KB | ###################################### | 100%
alabaster-0.7.11     |   17 KB | ###################################### | 100%
babel-2.6.0          |  5.7 MB | ###################################### | 100%
scikit-learn-0.19.1  |  4.6 MB | ###################################### | 100%
html5lib-1.0.1       |  183 KB | ###################################### | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: - DEBUG menuinst_win32:__init__(196): Menu: name: 'Anaconda${PY_VER} ${PLATFORM}', prefix: 'C:\ProgramData\Anaconda3\envs\tutorial', env_name: 'tutorial', mode: 'system', used_mode: 'system'
DEBUG menuinst_win32:create(320): Shortcut cmd is C:\ProgramData\Anaconda3\pythonw.exe, args are ['C:\\ProgramData\\Anaconda3\\cwp.py', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial\\pythonw.exe', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial\\Scripts\\spyder-script.py']
DEBUG menuinst_win32:create(320): Shortcut cmd is C:\ProgramData\Anaconda3\python.exe, args are ['C:\\ProgramData\\Anaconda3\\cwp.py', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial\\python.exe', 'C:\\ProgramData\\Anaconda3\\envs\\tutorial\\Scripts\\spyder-script.py', '--reset']
done
#
# To activate this environment, use
#
#     $ conda activate tutorial
#
# To deactivate an active environment, use
#
#     $ conda deactivate


(base) C:\Windows\system32>conda activate tutorial

(tutorial) C:\Windows\system32>pip install tensorflow
Collecting tensorflow
  Downloading https://files.pythonhosted.org/packages/0e/2a/c3fe6035f0a8726e5b210680af3ccaf826f4a64ce7306e57017aba749447/tensorflow-1.10.0-cp36-cp36m-win_amd64.
whl (37.7MB)
    100% |████████████████████████████████| 37.7MB 364kB/s
Collecting tensorboard<1.11.0,>=1.10.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/c6/17/ecd918a004f297955c30b4fffbea100b1606c225dbf0443264012773c3ff/tensorboard-1.10.0-py3-none-any.whl (3.3MB)
    100% |████████████████████████████████| 3.3MB 4.3MB/s
Collecting numpy<=1.14.5,>=1.13.3 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/0d/b7/0c804e0bcba6505f8392d042d5e333a5e06f308e019517111fbc7767a0bc/numpy-1.14.5-cp36-none-win_amd64.whl (13.4MB)
    100% |████████████████████████████████| 13.4MB 2.6MB/s
Collecting gast>=0.2.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/5c/78/ff794fcae2ce8aa6323e789d1f8b3b7765f601e7702726f430e814822b96/gast-0.2.0.tar.gz
Collecting absl-py>=0.1.6 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/a7/86/67f55488ec68982270142c340cd23cd2408835dc4b24bd1d1f1e114f24c3/absl-py-0.4.1.tar.gz (88kB)
    100% |████████████████████████████████| 92kB 1.4MB/s
Collecting setuptools<=39.1.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/8c/10/79282747f9169f21c053c562a0baa21815a8c7879be97abd930dbcf862e8/setuptools-39.1.0-py2.py3-none-any.whl
(566kB)
    100% |████████████████████████████████| 573kB 3.4MB/s
Collecting protobuf>=3.6.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/e8/df/d606d07cff0fc8d22abcc54006c0247002d11a7f2d218eb008d48e76851d/protobuf-3.6.1-cp36-cp36m-win_amd64.whl
 (1.1MB)
    100% |████████████████████████████████| 1.1MB 4.9MB/s
Collecting grpcio>=1.8.6 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/65/da/03e722b7981ab3222f292f735a3c157b1d1bca120c479d7e273273828170/grpcio-1.14.2-cp36-cp36m-win_amd64.whl
(1.5MB)
    100% |████████████████████████████████| 1.5MB 5.4MB/s
Requirement already satisfied: wheel>=0.26 in c:\programdata\anaconda3\envs\tutorial\lib\site-packages (from tensorflow) (0.31.1)
Requirement already satisfied: six>=1.10.0 in c:\programdata\anaconda3\envs\tutorial\lib\site-packages (from tensorflow) (1.11.0)
Collecting astor>=0.6.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/35/6b/11530768cac581a12952a2aad00e1526b89d242d0b9f59534ef6e6a1752f/astor-0.7.1-py2.py3-none-any.whl
Collecting termcolor>=1.1.0 (from tensorflow)
  Downloading https://files.pythonhosted.org/packages/8a/48/a76be51647d0eb9f10e2a4511bf3ffb8cc1e6b14e9e4fab46173aa79f981/termcolor-1.1.0.tar.gz
Collecting werkzeug>=0.11.10 (from tensorboard<1.11.0,>=1.10.0->tensorflow)
  Downloading https://files.pythonhosted.org/packages/20/c4/12e3e56473e52375aa29c4764e70d1b8f3efa6682bef8d0aae04fe335243/Werkzeug-0.14.1-py2.py3-none-any.whl (3
22kB)
    100% |████████████████████████████████| 327kB 403kB/s
Collecting markdown>=2.6.8 (from tensorboard<1.11.0,>=1.10.0->tensorflow)
  Downloading https://files.pythonhosted.org/packages/6d/7d/488b90f470b96531a3f5788cf12a93332f543dbab13c423a5e7ce96a0493/Markdown-2.6.11-py2.py3-none-any.whl (7
8kB)
    100% |████████████████████████████████| 81kB 1.1MB/s
Building wheels for collected packages: gast, absl-py, termcolor
  Running setup.py bdist_wheel for gast ... done
  Stored in directory: C:\Users\KOSTA\AppData\Local\pip\Cache\wheels\9a\1f\0e\3cde98113222b853e98fc0a8e9924480a3e25f1b4008cedb4f
  Running setup.py bdist_wheel for absl-py ... done
  Stored in directory: C:\Users\KOSTA\AppData\Local\pip\Cache\wheels\78\a3\a3\689120b95c26b9a21be6584b4b482b0fda0a1b60efd30af558
  Running setup.py bdist_wheel for termcolor ... done
  Stored in directory: C:\Users\KOSTA\AppData\Local\pip\Cache\wheels\7c\06\54\bc84598ba1daf8f970247f550b175aaaee85f68b4b0c5ab2c6
Successfully built gast absl-py termcolor
mkl-random 1.0.1 requires cython, which is not installed.
mkl-fft 1.0.4 requires cython, which is not installed.
Installing collected packages: werkzeug, numpy, markdown, setuptools, protobuf,
tensorboard, gast, absl-py, grpcio, astor, termcolor, tensorflow
  Found existing installation: numpy 1.15.1
    Uninstalling numpy-1.15.1:
      Successfully uninstalled numpy-1.15.1
  Found existing installation: setuptools 40.2.0
    Uninstalling setuptools-40.2.0:
      Successfully uninstalled setuptools-40.2.0
Successfully installed absl-py-0.4.1 astor-0.7.1 gast-0.2.0 grpcio-1.14.2 markdo
wn-2.6.11 numpy-1.14.5 protobuf-3.6.1 setuptools-39.1.0 tensorboard-1.10.0 tenso
rflow-1.10.0 termcolor-1.1.0 werkzeug-0.14.1
You are using pip version 10.0.1, however version 18.0 is available.
You should consider upgrading via the 'python -m pip install --upgrade pip' comm
and.

(tutorial) C:\Windows\system32>
~~~
~~~
(tutorial) C:\Windows\system32>python
Python 3.6.6 |Anaconda, Inc.| (default, Jun 28 2018, 11:27:44) [MSC v.1900 64 bi
t (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import tensorflow as tf
>>> print(tf.__version__)
1.10.0
>>> quit
Use quit() or Ctrl-Z plus Return to exit
>>> quit()

(tutorial) C:\Windows\system32>
~~~
~~~
(tutorial) C:\Windows\system32>pip install keras
Collecting keras
  Downloading https://files.pythonhosted.org/packages/34/7d/b1dedde8af99bd82f20e
d7e9697aac0597de3049b1f786aa2aac3b9bd4da/Keras-2.2.2-py2.py3-none-any.whl (299kB
)
    100% |████████████████████████████████| 307kB 839kB/s
Requirement already satisfied: six>=1.9.0 in c:\programdata\anaconda3\envs\tutor
ial\lib\site-packages (from keras) (1.11.0)
Requirement already satisfied: h5py in c:\programdata\anaconda3\envs\tutorial\li
b\site-packages (from keras) (2.8.0)
Collecting keras-applications==1.0.4 (from keras)
  Downloading https://files.pythonhosted.org/packages/54/90/8f327deaa37a71caddb5
9b7b4aaa9d4b3e90c0e76f8c2d1572005278ddc5/Keras_Applications-1.0.4-py2.py3-none-a
ny.whl (43kB)
    100% |████████████████████████████████| 51kB 1.2MB/s
Collecting pyyaml (from keras)
  Downloading https://files.pythonhosted.org/packages/4f/ca/5fad249c5032270540c2
4d2189b0ddf1396aac49b0bdc548162edcf14131/PyYAML-3.13-cp36-cp36m-win_amd64.whl (2
06kB)
    100% |████████████████████████████████| 215kB 975kB/s
Collecting keras-preprocessing==1.0.2 (from keras)
  Downloading https://files.pythonhosted.org/packages/71/26/1e778ebd737032749824
d5cba7dbd3b0cf9234b87ab5ec79f5f0403ca7e9/Keras_Preprocessing-1.0.2-py2.py3-none-
any.whl
Requirement already satisfied: numpy>=1.9.1 in c:\programdata\anaconda3\envs\tut
orial\lib\site-packages (from keras) (1.14.5)
Requirement already satisfied: scipy>=0.14 in c:\programdata\anaconda3\envs\tuto
rial\lib\site-packages (from keras) (1.1.0)
mkl-random 1.0.1 requires cython, which is not installed.
mkl-fft 1.0.4 requires cython, which is not installed.
Installing collected packages: keras-applications, pyyaml, keras-preprocessing,
keras
Successfully installed keras-2.2.2 keras-applications-1.0.4 keras-preprocessing-
1.0.2 pyyaml-3.13
You are using pip version 10.0.1, however version 18.0 is available.
You should consider upgrading via the 'python -m pip install --upgrade pip' comm
and.

(tutorial) C:\Windows\system32>
(tutorial) C:\Windows\system32>python
Python 3.6.6 |Anaconda, Inc.| (default, Jun 28 2018, 11:27:44) [MSC v.1900 64 bi
t (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import keras
Using TensorFlow backend.
>>> quit()

(tutorial) C:\Windows\system32>
~~~

~~~
(tutorial) C:\Windows\system32>deactivate

(base) C:\Windows\system32>conda create -n tutorial py

(base) C:\Windows\system32>conda create -n tutorial python=3.6 numpy scipy matpl
otlib spyder pandas seaborn scikit-learn h5py

(base) C:\Windows\system32>conda-env list
# conda environments:
#
base                  *  C:\ProgramData\Anaconda3
tutorial                 C:\ProgramData\Anaconda3\envs\tutorial


(base) C:\Windows\system32>conda-env delete tutorial
usage: conda-env [-h] {attach,create,export,list,remove,upload,update} ...
conda-env: error: invalid choice: 'delete' (choose from 'attach', 'create', 'exp
ort', 'list', 'remove', 'upload', 'update')

(base) C:\Windows\system32>conda-env remove tutorial
usage: conda-env [-h] {attach,create,export,list,remove,upload,update} ...
conda-env: error: unrecognized arguments: tutorial

(base) C:\Windows\system32>conda-env remove -n tutorial

Remove all packages in environment C:\ProgramData\Anaconda3\envs\tutorial:


## Package Plan ##

  environment location: C:\ProgramData\Anaconda3\envs\tutorial


The following packages will be REMOVED:

    alabaster:                0.7.11-py36_0
    asn1crypto:               0.24.0-py36_0
    astroid:                  2.0.4-py36_0
    babel:                    2.6.0-py36_0
    backcall:                 0.1.0-py36_0
    blas:                     1.0-mkl
    bleach:                   2.1.4-py36_0
    ca-certificates:          2018.03.07-0
    certifi:                  2018.8.24-py36_1
    cffi:                     1.11.5-py36h74b6da3_1
    chardet:                  3.0.4-py36_1
    cloudpickle:              0.5.5-py36_0
    colorama:                 0.3.9-py36h029ae33_0
    cryptography:             2.3.1-py36h74b6da3_0
    cycler:                   0.10.0-py36h009560c_0
    decorator:                4.3.0-py36_0
    docutils:                 0.14-py36h6012d8f_0
    entrypoints:              0.2.3-py36_2
    freetype:                 2.9.1-ha9979f8_1
    h5py:                     2.8.0-py36h3bdd7fb_2
    hdf5:                     1.10.2-hac2f561_1
    html5lib:                 1.0.1-py36_0
    icc_rt:                   2017.0.4-h97af966_0
    icu:                      58.2-ha66f8fd_1
    idna:                     2.7-py36_0
    imagesize:                1.1.0-py36_0
    intel-openmp:             2018.0.3-0
    ipykernel:                4.9.0-py36_0
    ipython:                  6.5.0-py36_0
    ipython_genutils:         0.2.0-py36h3c5d0ee_0
    isort:                    4.3.4-py36_0
    jedi:                     0.12.1-py36_0
    jinja2:                   2.10-py36_0
    jpeg:                     9b-hb83a4c4_2
    jsonschema:               2.6.0-py36h7636477_0
    jupyter_client:           5.2.3-py36_0
    jupyter_core:             4.4.0-py36_0
    keyring:                  13.2.1-py36_0
    kiwisolver:               1.0.1-py36h6538335_0
    lazy-object-proxy:        1.3.1-py36hfa6e2cd_2
    libpng:                   1.6.34-h79bbb47_0
    libsodium:                1.0.16-h9d3ae62_0
    markupsafe:               1.0-py36hfa6e2cd_1
    matplotlib:               2.2.3-py36hd159220_0
    mccabe:                   0.6.1-py36_1
    mistune:                  0.8.3-py36hfa6e2cd_1
    mkl:                      2018.0.3-1
    mkl_fft:                  1.0.4-py36h1e22a9b_1
    mkl_random:               1.0.1-py36h77b88f5_1
    nbconvert:                5.3.1-py36_0
    nbformat:                 4.4.0-py36h3a5bc1b_0
    numpy:                    1.15.1-py36ha559c80_0
    numpy-base:               1.15.1-py36h8128ebf_0
    numpydoc:                 0.8.0-py36_0
    openssl:                  1.0.2p-hfa6e2cd_0
    packaging:                17.1-py36_0
    pandas:                   0.23.4-py36h830ac7b_0
    pandoc:                   2.2.3.2-0
    pandocfilters:            1.4.2-py36_1
    parso:                    0.3.1-py36_0
    patsy:                    0.5.0-py36_0
    pickleshare:              0.7.4-py36h9de030f_0
    pip:                      10.0.1-py36_0
    prompt_toolkit:           1.0.15-py36h60b8f86_0
    psutil:                   5.4.7-py36hfa6e2cd_0
    pycodestyle:              2.4.0-py36_0
    pycparser:                2.18-py36_1
    pyflakes:                 2.0.0-py36_0
    pygments:                 2.2.0-py36hb010967_0
    pylint:                   2.1.1-py36_0
    pyopenssl:                18.0.0-py36_0
    pyparsing:                2.2.0-py36_1
    pyqt:                     5.9.2-py36ha878b3d_0
    pysocks:                  1.6.8-py36_0
    python:                   3.6.6-hea74fb7_0
    python-dateutil:          2.7.3-py36_0
    pytz:                     2018.5-py36_0
    pywin32:                  223-py36hfa6e2cd_1
    pyzmq:                    17.1.2-py36hfa6e2cd_0
    qt:                       5.9.6-vc14h62aca36_0
    qtawesome:                0.4.4-py36h5aa48f6_0
    qtconsole:                4.4.1-py36_0
    qtpy:                     1.5.0-py36_0
    requests:                 2.19.1-py36_0
    rope:                     0.11.0-py36_0
    scikit-learn:             0.19.1-py36hae9bb9f_0
    scipy:                    1.1.0-py36h4f6bf74_1
    seaborn:                  0.9.0-py36_0
    setuptools:               40.2.0-py36_0
    simplegeneric:            0.8.1-py36_2
    sip:                      4.19.12-py36h6538335_0
    six:                      1.11.0-py36_1
    snowballstemmer:          1.2.1-py36h763602f_0
    sphinx:                   1.7.8-py36_0
    sphinxcontrib:            1.0-py36_1
    sphinxcontrib-websupport: 1.1.0-py36_1
    spyder:                   3.3.1-py36_1
    spyder-kernels:           0.2.6-py36_0
    sqlite:                   3.24.0-h7602738_0
    statsmodels:              0.9.0-py36h452e1ab_0
    testpath:                 0.3.1-py36h2698cfe_0
    tornado:                  5.1-py36hfa6e2cd_0
    traitlets:                4.3.2-py36h096827d_0
    typed-ast:                1.1.0-py36hfa6e2cd_0
    urllib3:                  1.23-py36_0
    vc:                       14-h0510ff6_3
    vs2015_runtime:           14.0.25123-3
    wcwidth:                  0.1.7-py36h3d5aa90_0
    webencodings:             0.5.1-py36_1
    wheel:                    0.31.1-py36_0
    win_inet_pton:            1.0.1-py36_1
    wincertstore:             0.2-py36h7fe50ca_0
    wrapt:                    1.10.11-py36hfa6e2cd_2
    zeromq:                   4.2.5-he025d50_1
    zlib:                     1.2.11-h8395fce_2

Proceed ([y]/n)? y


(base) C:\Windows\system32>
~~~
