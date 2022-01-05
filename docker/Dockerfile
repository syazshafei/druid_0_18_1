FROM openjdk:8-jdk

# Druid installation
RUN mkdir -p /home/druid
WORKDIR /home/druid
COPY apache-druid-0.18.1-bin.tar.gz apache-druid-0.18.1-bin.tar.gz
RUN tar -xzf apache-druid-0.18.1-bin.tar.gz
RUN rm -f apache-druid-0.18.1-bin.tar.gz

WORKDIR /home/druid/apache-druid-0.18.1
 
EXPOSE 2181 2888 3888
EXPOSE 8081
EXPOSE 8082
EXPOSE 8083
EXPOSE 8091
EXPOSE 8090
EXPOSE 8888

CMD ["./bin/start-micro-quickstart"]