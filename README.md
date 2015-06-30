# InstallZookeeper

# download and extract zookeeper
```shell
cd /opt && wget http://www.apache.org/dist/zookeeper/zookeeper-3.3.3/zookeeper-3.3.3.tar.gz
tar zxf zookeeper-3.3.6.tar.gz 
```
# configure
* I install zookeeper as root
```shell
cd zookeeper-3.3.6/conf
cp zoo_sample.cfg zoo.cfg
mkdir -p root/data
vi zoo.cfg
  -edit dataDir=/root/data
```

# run
```shell
cd /opt/zookeeper-3.3.6/bin
./zkServer.sh start
```
