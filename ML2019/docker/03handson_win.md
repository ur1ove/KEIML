### 도커 핸즈온
- 도커 버전 확인
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker --version
Docker version 18.09.1, build 4c52b90
~~~
- 도커 정보 확인
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker info
Containers: 0
 Running: 0
 Paused: 0
 Stopped: 0
Images: 0
Server Version: 18.09.1
Storage Driver: overlay2
 Backing Filesystem: extfs
 Supports d_type: true
 Native Overlay Diff: true
Logging Driver: json-file
Cgroup Driver: cgroupfs
Plugins:
 Volume: local
 Network: bridge host macvlan null overlay
 Log: awslogs fluentd gcplogs gelf journald json-file local logentries splunk syslog
Swarm: inactive
Runtimes: runc
Default Runtime: runc
Init Binary: docker-init
containerd version: 9754871865f7fe2f4e74d43e2fc7ccd237edcbce
runc version: 96ec2177ae841256168fcf76954f7177af9446eb
init version: fec3683
Security Options:
 seccomp
  Profile: default
Kernel Version: 4.9.125-linuxkit
Operating System: Docker for Windows
OSType: linux
Architecture: x86_64
CPUs: 2
Total Memory: 1.934GiB
Name: linuxkit-00155d963401
ID: KIKS:EVWQ:34SI:FC43:2WJV:B5UR:7RWT:SFQJ:NVU3:PONZ:67YH:IIZL
Docker Root Dir: /var/lib/docker
Debug Mode (client): false
Debug Mode (server): true
 File Descriptors: 22
 Goroutines: 46
 System Time: 2019-01-29T12:06:37.7547954Z
 EventsListeners: 1
Registry: https://index.docker.io/v1/
Labels:
Experimental: false
Insecure Registries:
 127.0.0.0/8
Live Restore Enabled: false
Product License: Community Engine
~~~
- 도커 처음 실행하기  
  (1) 대문자 사용이 안 되고  
  (2) 도커 허브에 등록된 이미지를 먼저 불러옴  
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker run firstDocker
docker: invalid reference format: repository name must be lowercase.
See 'docker run --help'.

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker run firstdocker
Unable to find image 'firstdocker:latest' locally
docker: Error response from daemon: pull access denied for firstdocker, repository does not exist or may require 'docker login'.
See 'docker run --help'.

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker run hello-world
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
1b930d010525: Pull complete
Digest: sha256:2557e3c07ed1e38f26e389462d03ed943586f744621577a99efb77324b0fe535
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/
~~~
- 도커 이미지, 컨테이너 확인
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker image ls
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
hello-world         latest              fce289e99eb9        4 weeks ago         1.84kB

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker container ls
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker ps -a
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS                     PORTS               NAMES
9927d5ed383b        hello-world         "/hello"            2 minutes ago       Exited (0) 2 minutes ago                       boring_austin

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker container ls -all
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS                     PORTS               NAMES
9927d5ed383b        hello-world         "/hello"            2 minutes ago       Exited (0) 2 minutes ago                       boring_austin
~~~
- 도커 컨테이너 삭제
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker rm 9927d5ed383b
9927d5ed383b

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker container ls -all
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
~~~
- 도커 이미지 삭제
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker image ls
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
hello-world         latest              fce289e99eb9        4 weeks ago         1.84kB

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker rmi fce289e99eb9
Untagged: hello-world:latest
Untagged: hello-world@sha256:2557e3c07ed1e38f26e389462d03ed943586f744621577a99efb77324b0fe535
Deleted: sha256:fce289e99eb9bca977dae136fbe2a82b6b7d4c372474c9235adc1741675f587e
Deleted: sha256:af0b15c8625bb1938f1d7b17081031f649fd14e6b233688eea3c5483994a66a3

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker image ls
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
~~~
