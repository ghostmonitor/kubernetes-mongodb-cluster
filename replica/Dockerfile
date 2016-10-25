# mongo-cluster
FROM mongo:3.2

EXPOSE 27017

RUN mkdir -p /opt/mongo/ && \
	apt-get update && apt-get -y upgrade && apt-get install -y netcat

COPY start_replica.sh /opt/mongo/

WORKDIR /opt/mongo
#USER mongodb

CMD /opt/mongo/start_replica.sh
