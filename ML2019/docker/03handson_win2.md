### 도커 핸즈온(2/4)  
  
- 웹서버 이미지 띄워보기(nginx)  
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker run --name nginx-test -p 8088:80 -d nginx
Unable to find image 'nginx:latest' locally
latest: Pulling from library/nginx
5e6ec7f28fb7: Pull complete
ab804f9bbcbe: Pull complete
052b395f16bc: Pull complete
Digest: sha256:56bcd35e8433343dbae0484ed5b740843dd8bff9479400990f251c13bbb94763
Status: Downloaded newer image for nginx:latest
a5d1d2faaa63064fd8d99eb581506340b46e6299fa6f9fe5aff22a69f3c883cc

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
nginx               latest              42b4762643dc        6 days ago          109MB

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker ps -all
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                  NAMES
a5d1d2faaa63        nginx               "nginx -g 'daemon of…"   12 minutes ago      Up 12 minutes       0.0.0.0:8088->80/tcp   nginx-test
~~~  
  
(1) 이 때, 보안 경고 창이 나오면 엑세스 허용을 클릭하자.  
![엑세스_허용.png](./imgs/엑세스_허용.png)  
(2) 웹브라우저에 [URL](http://localhost:8088) 을 확인한다.  
![웹서버_확인.png](./imgs/웹서버_확인.png)  
  
- 컨테이너 종료 / 삭제  
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker stop nginx-test
nginx-test

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker rm nginx-test
nginx-test

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
nginx               latest              42b4762643dc        6 days ago          109MB
~~~
- 도커 이미지 다운로드  
~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker pull ubuntu
Using default tag: latest
latest: Pulling from library/ubuntu
38e2e6cd5626: Pull complete
705054bc3f5b: Pull complete
c7051e069564: Pull complete
7308e914506c: Pull complete
Digest: sha256:945039273a7b927869a07b375dc3148de16865de44dec8398672977e050a072e
Status: Downloaded newer image for ubuntu:latest

(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
nginx               latest              42b4762643dc        6 days ago          109MB
ubuntu              latest              20bb25d32758        6 days ago          87.5MB
~~~

~~~
(base) E:\Data\블록체인\뷰티풀체인\dockerHandsOn>docker run --name nginx-test -p 8088:80 -it ubuntu /bin/bash
root@27740523e18c:/# apt update
root@27740523e18c:/# apt update
Get:1 http://archive.ubuntu.com/ubuntu bionic InRelease [242 kB]
Get:2 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
Get:3 http://archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
Get:4 http://archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB]
Get:5 http://archive.ubuntu.com/ubuntu bionic/restricted amd64 Packages [13.5 kB]
Get:6 http://archive.ubuntu.com/ubuntu bionic/multiverse amd64 Packages [186 kB]
Get:7 http://security.ubuntu.com/ubuntu bionic-security/universe amd64 Packages [140 kB]
Get:8 http://archive.ubuntu.com/ubuntu bionic/universe amd64 Packages [11.3 MB]
Get:9 http://security.ubuntu.com/ubuntu bionic-security/main amd64 Packages [315 kB]
Get:10 http://security.ubuntu.com/ubuntu bionic-security/multiverse amd64 Packages [3451 B]
Get:11 http://archive.ubuntu.com/ubuntu bionic/main amd64 Packages [1344 kB]
Get:12 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 Packages [645 kB]
Get:13 http://archive.ubuntu.com/ubuntu bionic-updates/universe amd64 Packages [912 kB]
Get:14 http://archive.ubuntu.com/ubuntu bionic-updates/multiverse amd64 Packages [6955 B]
Get:15 http://archive.ubuntu.com/ubuntu bionic-updates/restricted amd64 Packages [10.7 kB]
Get:16 http://archive.ubuntu.com/ubuntu bionic-backports/universe amd64 Packages [3666 B]
Fetched 15.4 MB in 16s (952 kB/s)
Reading package lists... Done
Building dependency tree
Reading state information... Done
All packages are up to date.
root@27740523e18c:/# apt install -y nginx
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
  fontconfig-config fonts-dejavu-core geoip-database iproute2 libatm1 libbsd0 libelf1 libexpat1 libfontconfig1 libfreetype6 libgd3 libgeoip1 libicu60 libjbig0 libjpeg-turbo8 libjpeg8 libmnl0
  libnginx-mod-http-geoip libnginx-mod-http-image-filter libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream libpng16-16 libssl1.1 libtiff5 libwebp6 libx11-6 libx11-data libxau6
  libxcb1 libxdmcp6 libxml2 libxpm4 libxslt1.1 libxtables12 multiarch-support nginx-common nginx-core ucf
Suggested packages:
  iproute2-doc libgd-tools geoip-bin fcgiwrap nginx-doc ssl-cert
The following NEW packages will be installed:
  fontconfig-config fonts-dejavu-core geoip-database iproute2 libatm1 libbsd0 libelf1 libexpat1 libfontconfig1 libfreetype6 libgd3 libgeoip1 libicu60 libjbig0 libjpeg-turbo8 libjpeg8 libmnl0
  libnginx-mod-http-geoip libnginx-mod-http-image-filter libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream libpng16-16 libssl1.1 libtiff5 libwebp6 libx11-6 libx11-data libxau6
  libxcb1 libxdmcp6 libxml2 libxpm4 libxslt1.1 libxtables12 multiarch-support nginx nginx-common nginx-core ucf
0 upgraded, 40 newly installed, 0 to remove and 0 not upgraded.
Need to get 16.9 MB of archives.
After this operation, 61.4 MB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu bionic/main amd64 multiarch-support amd64 2.27-3ubuntu1 [6916 B]
Get:2 http://archive.ubuntu.com/ubuntu bionic/main amd64 libxau6 amd64 1:1.0.8-1 [8376 B]
Get:3 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libjpeg-turbo8 amd64 1.5.2-0ubuntu5.18.04.1 [110 kB]
Get:4 http://archive.ubuntu.com/ubuntu bionic/main amd64 libelf1 amd64 0.170-0.4 [44.1 kB]
Get:5 http://archive.ubuntu.com/ubuntu bionic/main amd64 libmnl0 amd64 1.0.4-2 [12.3 kB]
Get:6 http://archive.ubuntu.com/ubuntu bionic/main amd64 iproute2 amd64 4.15.0-2ubuntu1 [721 kB]
Get:7 http://archive.ubuntu.com/ubuntu bionic/main amd64 libatm1 amd64 1:2.5.1-2build1 [21.9 kB]
Get:8 http://archive.ubuntu.com/ubuntu bionic/main amd64 libbsd0 amd64 0.8.7-1 [41.5 kB]
Get:9 http://archive.ubuntu.com/ubuntu bionic/main amd64 libexpat1 amd64 2.2.5-3 [80.2 kB]
Get:10 http://archive.ubuntu.com/ubuntu bionic/main amd64 libicu60 amd64 60.2-3ubuntu3 [8054 kB]
Get:10 http://archive.ubuntu.com/ubuntu bionic/main amd64 libicu60 amd64 60.2-3ubuntu3 [8054 kB]

~~~
