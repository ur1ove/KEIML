### 설치 잘 안 되지요?
- 
~~~
출처 : https://github.com/tensorflow/tensorflow/issues/22794 답글에서 https://www.pugetsystems.com/labs/hpc/The-Best-Way-to-Install-TensorFlow-with-GPU-Support-on-Windows-10-Without-Installing-CUDA-1187/
conda create --name tf-gpu
conda install -c aaronzs tensorflow-gpu
conda install -c anaconda cudatoolkit
conda install -c anaconda cudnn
conda install keras-gpu
~~~
- 이도 잘 안되서 
~~~
(kerasGPU) D:\Data\kerasGPU\download>conda install -c anaconda cudatoolkit
Solving environment: done

## Package Plan ##

  environment location: C:\ProgramData\Anaconda3\envs\kerasGPU

  added / updated specs:
    - cudatoolkit


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    cudatoolkit-9.0            |                1       339.8 MB  anaconda

The following packages will be UPDATED:

    certifi:        2018.10.15-py36_0                                        --> 2018.10.15-py36_0 anaconda
    cudatoolkit:    9.0-1                  file:///D:/Data/kerasGPU/download --> 9.0-1             anaconda
    vs2015_runtime: 14.15.26706-h3a45250_0                                   --> 15.5.2-3          anaconda

The following packages will be DOWNGRADED:

    vc:             14.1-h0510ff6_4                                          --> 14.1-h21ff451_3   anaconda

Proceed ([y]/n)? y


Downloading and Extracting Packages
cudatoolkit-9.0      | 339.8 MB  | #####9                                                   |  11%

CondaHTTPError: HTTP 000 CONNECTION FAILED for url <https://conda.anaconda.org/anaconda/win-64/cudat
oolkit-9.0-1.tar.bz2>
Elapsed: -

An HTTP error occurred when trying to retrieve this URL.
HTTP errors are often intermittent, and a simple retry will get you on your way.




(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\Program Files\Java\jdk1.8.0_112"

(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME_CONDA_BACKUP=C:\Program Files\Java\jdk1.8.0_112"


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\ProgramData\Anaconda3\envs\kerasGPU\Library"


(kerasGPU) D:\Data\kerasGPU\download>
~~~

https://anaconda.org/anaconda/cudatoolkit/files

~~~
(kerasGPU) D:\Data\kerasGPU\download>conda install -c anaconda certifi
Solving environment: done

## Package Plan ##

  environment location: C:\ProgramData\Anaconda3\envs\kerasGPU

  added / updated specs:
    - certifi


The following packages will be UPDATED:

    certifi:        2018.10.15-py36_0      --> 2018.10.15-py36_0 anaconda
    vs2015_runtime: 14.15.26706-h3a45250_0 --> 15.5.2-3          anaconda

The following packages will be DOWNGRADED:

    vc:             14.1-h0510ff6_4        --> 14.1-h21ff451_3   anaconda

Proceed ([y]/n)? y

Preparing transaction: done
Verifying transaction: done
Executing transaction: done

(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\Program Files\Java\jdk1.8.0_112"

(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME_CONDA_BACKUP=C:\Program Files\Java\jdk1.8.0_112"


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\ProgramData\Anaconda3\envs\kerasGPU\Library"


(kerasGPU) D:\Data\kerasGPU\download>conda install -c anaconda certifi
Solving environment: done

# All requested packages already installed.


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\Program Files\Java\jdk1.8.0_112"

(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME_CONDA_BACKUP=C:\Program Files\Java\jdk1.8.0_112"


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\ProgramData\Anaconda3\envs\kerasGPU\Library"


(kerasGPU) D:\Data\kerasGPU\download>
~~~
~~~
(kerasGPU) D:\Data\kerasGPU\download>conda install -c anaconda cudnn
Solving environment: done

## Package Plan ##

  environment location: C:\ProgramData\Anaconda3\envs\kerasGPU

  added / updated specs:
    - cudnn


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    cudnn-7.1.4                |        cuda9.0_0       192.3 MB  anaconda

The following packages will be UPDATED:

    cudnn: 7.1.4-cuda9.0_0 <unknown> --> 7.1.4-cuda9.0_0 anaconda

Proceed ([y]/n)? n


CondaSystemExit: Exiting.


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\Program Files\Java\jdk1.8.0_112"

(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME_CONDA_BACKUP=C:\Program Files\Java\jdk1.8.0_112"


(kerasGPU) D:\Data\kerasGPU\download>set "JAVA_HOME=C:\ProgramData\Anaconda3\envs\kerasGPU\Library"


(kerasGPU) D:\Data\kerasGPU\download>
~~~
