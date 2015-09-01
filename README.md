# zookeeper-env
搭建zookeeper集群，最少三台机器


在zoo.cfg目录中需要注意  
dataDir=/home/work/data/zookeeper
clientPort=11000  通信端口

server.0=ip1:11010:11011  
server.1=ip2:11010:11011  
server.2=ip3:11010:11011  


必须  
pc1 ip1机器的dataDir目录 创建myid并赋值0,因为server.0  
pc2 ip2机器的dataDir目录 创建myid并赋值1,因为server.1  
pc3 ip3机器的dataDir目录 创建myid并赋值2,因为server.2  




启动
直接使用
./bin/zkServer start


查询状态
./bin/zkServer status






