### GeoPandas 설치
- [http://geopandas.org/install.html](http://geopandas.org/install.html)
~~~
Last login: Tue Dec 25 18:54:02 on ttys000
Benjaminui-MacBook-Pro:~ bEnnY$ source activate geopandas
(geopandas) Benjaminui-MacBook-Pro:~ bEnnY$ conda install -c conda-forge geopandas
Fetching package metadata ...........
Solving package specifications: .

Package plan for installation in environment /Users/bEnnY/anaconda/envs/geopandas:

The following NEW packages will be INSTALLED:

    attrs:           18.2.0-py_0                conda-forge
    blas:            1.0-mkl                               
    boost-cpp:       1.68.0-h6f8c590_1000       conda-forge
    bzip2:           1.0.6-h1de35cc_1002        conda-forge
    ca-certificates: 2018.11.29-ha4d7672_0      conda-forge
    cairo:           1.14.12-h9d4d9ac_1005      conda-forge
    certifi:         2018.11.29-py36_1000       conda-forge
    click:           7.0-py_0                   conda-forge
    click-plugins:   1.0.4-py_0                 conda-forge
    cligj:           0.5.0-py_0                 conda-forge
    curl:            7.63.0-heae2a1f_1000       conda-forge
    cycler:          0.10.0-py_1                conda-forge
    descartes:       1.1.0-py_2                 conda-forge
    expat:           2.2.5-h0a44026_1002        conda-forge
    fiona:           1.8.4-py36h0e3174d_1002    conda-forge
    fontconfig:      2.13.1-h1e4e890_1000       conda-forge
    freetype:        2.9.1-h597ad8a_1005        conda-forge
    freexl:          1.0.5-h1de35cc_1002        conda-forge
    gdal:            2.4.0-py36h8e9a8e4_1000    conda-forge
    geopandas:       0.4.0-py_1                 conda-forge
    geos:            3.7.0-h0a44026_1000        conda-forge
    geotiff:         1.4.3-hce09ea4_1000        conda-forge
    gettext:         0.19.8.1-hcca000d_1001     conda-forge
    giflib:          5.1.4-h1de35cc_1001        conda-forge
    glib:            2.56.2-h67dad55_1001       conda-forge
    hdf4:            4.2.13-hf3c6af0_1002       conda-forge
    hdf5:            1.10.4-nompi_h5598ddc_1105 conda-forge
    icu:             58.2-h0a44026_1000         conda-forge
    jpeg:            9c-h1de35cc_1001           conda-forge
    json-c:          0.13.1-h1de35cc_1001       conda-forge
    kealib:          1.4.10-hf5ed860_1002       conda-forge
    kiwisolver:      1.0.1-py36h04f5b5a_1002    conda-forge
    krb5:            1.16.3-h24a3359_1000       conda-forge
    libcurl:         7.63.0-h76de61e_1000       conda-forge
    libcxx:          7.0.0-h2d50403_2           conda-forge
    libdap4:         3.19.1-hae55d67_1000       conda-forge
    libedit:         3.1.20170329-hcfe32e1_1001 conda-forge
    libffi:          3.2.1-h0a44026_1005        conda-forge
    libgdal:         2.4.0-hbb94375_1000        conda-forge
    libgfortran:     3.0.0-1001                 conda-forge
    libiconv:        1.15-h1de35cc_1004         conda-forge
    libkml:          1.3.0-h71ee1b2_1009        conda-forge
    libnetcdf:       4.6.2-h6b88ef6_1001        conda-forge
    libpng:          1.6.36-ha441bb4_1000       conda-forge
    libpq:           10.6-hbe1e24e_1000         conda-forge
    libspatialindex: 1.8.5-h0a44026_1003        conda-forge
    libspatialite:   4.3.0a-hc5068f1_1025       conda-forge
    libssh2:         1.8.0-hf30b1f0_1003        conda-forge
    libtiff:         4.0.10-h79f4b77_1001       conda-forge
    libxml2:         2.9.8-hf14e9c8_1005        conda-forge
    llvm-meta:       7.0.0-0                    conda-forge
    matplotlib:      2.2.3-py36h0e0179f_0       conda-forge
    mkl:             2017.0.3-0                            
    munch:           2.3.2-py_0                 conda-forge
    ncurses:         6.1-h0a44026_1002          conda-forge
    numpy:           1.13.1-py36_0                         
    openjpeg:        2.3.0-h3bf0609_1003        conda-forge
    openssl:         1.0.2p-h1de35cc_1002       conda-forge
    pandas:          0.23.4-py36h1702cab_1000   conda-forge
    pcre:            8.41-h0a44026_1003         conda-forge
    pip:             18.1-py36_1000             conda-forge
    pixman:          0.34.0-h1de35cc_1003       conda-forge
    poppler:         0.67.0-hf4bf5f7_1002       conda-forge
    poppler-data:    0.4.9-1                    conda-forge
    postgresql:      10.6-ha1bbaa7_1000         conda-forge
    proj4:           5.2.0-h1de35cc_1001        conda-forge
    psycopg2:        2.7.6.1-py36hdbc3d79_1000  conda-forge
    pyparsing:       2.3.1-py_0                 conda-forge
    pyproj:          1.9.6-py36h9c430a6_1000    conda-forge
    pysal:           1.14.4.post2-py36_1001     conda-forge
    python:          3.6.7-h4a56312_1001        conda-forge
    python-dateutil: 2.7.5-py_0                 conda-forge
    pytz:            2018.9-py_0                conda-forge
    readline:        7.0-hcfe32e1_1001          conda-forge
    rtree:           0.8.3-py36_1000            conda-forge
    scipy:           0.19.1-np113py36_0                    
    setuptools:      40.6.3-py36_0              conda-forge
    shapely:         1.6.4-py36h1d95287_1001    conda-forge
    six:             1.12.0-py36_1000           conda-forge
    sqlalchemy:      1.2.16-py36h1de35cc_1000   conda-forge
    sqlite:          3.26.0-h1765d9f_1000       conda-forge
    tk:              8.6.9-ha441bb4_1000        conda-forge
    tornado:         5.1.1-py36h1de35cc_1000    conda-forge
    tzcode:          2018g-h1de35cc_1001        conda-forge
    wheel:           0.32.3-py36_0              conda-forge
    xerces-c:        3.2.2-h44e365a_1001        conda-forge
    xz:              5.2.4-h1de35cc_1001        conda-forge
    zlib:            1.2.11-h1de35cc_1004       conda-forge

Proceed ([y]/n)?  y

bzip2-1.0.6-h1 100% |################################| Time: 0:00:00   1.45 MB/s
ca-certificate 100% |################################| Time: 0:00:00   1.61 MB/s
freexl-1.0.5-h 100% |################################| Time: 0:00:00   8.32 MB/s
giflib-5.1.4-h 100% |################################| Time: 0:00:00   2.65 MB/s
jpeg-9c-h1de35 100% |################################| Time: 0:00:00   3.19 MB/s
json-c-0.13.1- 100% |################################| Time: 0:00:00   4.94 MB/s
libgfortran-3. 100% |################################| Time: 0:00:00   4.72 MB/s
libiconv-1.15- 100% |################################| Time: 0:00:00   3.54 MB/s
llvm-meta-7.0. 100% |################################| Time: 0:00:00   1.96 MB/s
pixman-0.34.0- 100% |################################| Time: 0:00:00   4.42 MB/s
poppler-data-0 100% |################################| Time: 0:00:01   3.24 MB/s
proj4-5.2.0-h1 100% |################################| Time: 0:00:03   1.93 MB/s
tzcode-2018g-h 100% |################################| Time: 0:00:00   2.31 MB/s
xz-5.2.4-h1de3 100% |################################| Time: 0:00:00   2.75 MB/s
zlib-1.2.11-h1 100% |################################| Time: 0:00:00   3.05 MB/s
hdf5-1.10.4-no 100% |################################| Time: 0:00:02   2.17 MB/s
libcxx-7.0.0-h 100% |################################| Time: 0:00:00   4.07 MB/s
libpng-1.6.36- 100% |################################| Time: 0:00:00   4.64 MB/s
openssl-1.0.2p 100% |################################| Time: 0:00:01   3.01 MB/s
tk-8.6.9-ha441 100% |################################| Time: 0:00:00   3.30 MB/s
expat-2.2.5-h0 100% |################################| Time: 0:00:00   3.39 MB/s
freetype-2.9.1 100% |################################| Time: 0:00:00   3.72 MB/s
geos-3.7.0-h0a 100% |################################| Time: 0:00:00   3.86 MB/s
hdf4-4.2.13-hf 100% |################################| Time: 0:00:00   4.57 MB/s
icu-58.2-h0a44 100% |################################| Time: 0:00:08   2.83 MB/s
kealib-1.4.10- 100% |################################| Time: 0:00:00   2.34 MB/s
libffi-3.2.1-h 100% |################################| Time: 0:00:00   2.99 MB/s
libspatialinde 100% |################################| Time: 0:00:00   3.24 MB/s
libssh2-1.8.0- 100% |################################| Time: 0:00:00   3.44 MB/s
libtiff-4.0.10 100% |################################| Time: 0:00:00   3.09 MB/s
ncurses-6.1-h0 100% |################################| Time: 0:00:00   3.37 MB/s
pcre-8.41-h0a4 100% |################################| Time: 0:00:00   4.20 MB/s
boost-cpp-1.68 100% |################################| Time: 0:00:09   2.11 MB/s
geotiff-1.4.3- 100% |################################| Time: 0:00:00   4.05 MB/s
gettext-0.19.8 100% |################################| Time: 0:00:00   4.77 MB/s
libedit-3.1.20 100% |################################| Time: 0:00:00   6.87 MB/s
libxml2-2.9.8- 100% |################################| Time: 0:00:00   4.19 MB/s
openjpeg-2.3.0 100% |################################| Time: 0:00:00   2.47 MB/s
readline-7.0-h 100% |################################| Time: 0:00:00   2.69 MB/s
xerces-c-3.2.2 100% |################################| Time: 0:00:00   3.65 MB/s
fontconfig-2.1 100% |################################| Time: 0:00:00   4.15 MB/s
glib-2.56.2-h6 100% |################################| Time: 0:00:01   2.64 MB/s
krb5-1.16.3-h2 100% |################################| Time: 0:00:00   3.10 MB/s
libkml-1.3.0-h 100% |################################| Time: 0:00:00   3.42 MB/s
libpq-10.6-hbe 100% |################################| Time: 0:00:01   2.03 MB/s
sqlite-3.26.0- 100% |################################| Time: 0:00:01   1.65 MB/s
cairo-1.14.12- 100% |################################| Time: 0:00:00   1.56 MB/s
libcurl-7.63.0 100% |################################| Time: 0:00:00   1.99 MB/s
libspatialite- 100% |################################| Time: 0:00:01   2.28 MB/s
postgresql-10. 100% |################################| Time: 0:00:01   3.21 MB/s
python-3.6.7-h 100% |################################| Time: 0:00:09   2.37 MB/s
attrs-18.2.0-p 100% |################################| Time: 0:00:00   2.10 MB/s
certifi-2018.1 100% |################################| Time: 0:00:00   2.05 MB/s
click-7.0-py_0 100% |################################| Time: 0:00:00   5.17 MB/s
curl-7.63.0-he 100% |################################| Time: 0:00:00   4.13 MB/s
kiwisolver-1.0 100% |################################| Time: 0:00:00   4.24 MB/s
psycopg2-2.7.6 100% |################################| Time: 0:00:00   1.19 MB/s
pyparsing-2.3. 100% |################################| Time: 0:00:00   3.03 MB/s
pytz-2018.9-py 100% |################################| Time: 0:00:00   2.71 MB/s
rtree-0.8.3-py 100% |################################| Time: 0:00:00   2.38 MB/s
six-1.12.0-py3 100% |################################| Time: 0:00:00   1.77 MB/s
sqlalchemy-1.2 100% |################################| Time: 0:00:00   3.22 MB/s
tornado-5.1.1- 100% |################################| Time: 0:00:00   3.13 MB/s
click-plugins- 100% |################################| Time: 0:00:00   8.48 MB/s
cligj-0.5.0-py 100% |################################| Time: 0:00:00   6.84 MB/s
cycler-0.10.0- 100% |################################| Time: 0:00:00   6.24 MB/s
libdap4-3.19.1 100% |################################| Time: 0:00:00   3.59 MB/s
libnetcdf-4.6. 100% |################################| Time: 0:00:00   3.78 MB/s
munch-2.3.2-py 100% |################################| Time: 0:00:00   8.15 MB/s
poppler-0.67.0 100% |################################| Time: 0:00:01   1.42 MB/s
pyproj-1.9.6-p 100% |################################| Time: 0:00:00   2.05 MB/s
python-dateuti 100% |################################| Time: 0:00:00   2.93 MB/s
setuptools-40. 100% |################################| Time: 0:00:00   2.40 MB/s
shapely-1.6.4- 100% |################################| Time: 0:00:00   2.26 MB/s
libgdal-2.4.0- 100% |################################| Time: 0:00:09   2.00 MB/s
matplotlib-2.2 100% |################################| Time: 0:00:01   3.95 MB/s
pandas-0.23.4- 100% |################################| Time: 0:00:04   2.23 MB/s
pysal-1.14.4.p 100% |################################| Time: 0:00:06   2.44 MB/s
wheel-0.32.3-p 100% |################################| Time: 0:00:00   3.68 MB/s
descartes-1.1. 100% |################################| Time: 0:00:00 513.69 kB/s
gdal-2.4.0-py3 100% |################################| Time: 0:00:01   1.32 MB/s
pip-18.1-py36_ 100% |################################| Time: 0:00:00   1.92 MB/s
fiona-1.8.4-py 100% |################################| Time: 0:00:00   2.23 MB/s
geopandas-0.4. 100% |################################| Time: 0:00:00   3.17 MB/s
~~~
