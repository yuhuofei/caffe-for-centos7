# Caff-for-centos7

this project can be cmake on cnetos 7 by using either atlas or mkl

first,  install mkl in /usr/local/, or yum install atlas, maybe you need to install epel repo first


second, to test mkl on centos 7
```shel
# in caffe root dir
mkdir build
cd build
cmake .. -DBLAS:string="mkl"
make -j32
```

to test atlas on centos 7
```shell
# in caffe root dir
mkdir build
cd build
cmake .. -DBLAS:string="atlas"
make -j32
```
