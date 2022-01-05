# Apache Druid 0.18.1 Installation Guide

Download Druid 0.18.1 Binary and put inside `docker` directory
```
curl https://www.apache.org/dyn/closer.cgi?path=/druid/0.18.1/apache-druid-0.18.1-bin.tar.gz --output apache-druid-0.18.1-bin.tar.gz
```


Build image
```
cd docker
sudo docker build -t apache-druid:0.18.1 .
```
Run container
```
sudo docker-compose up -d
```
If make changes to Druid configuration, restart Druid container
```
sudo docker restart druid
```
Stop container
```
sudo docker-compose down
```
