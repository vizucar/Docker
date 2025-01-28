FROM mongo:latest
COPY vizucar-bdd.json /vizucar-bdd.json
COPY data-init.sh /docker-entrypoint-initdb.d/init-data.sh
RUN chmod +x /docker-entrypoint-initdb.d/init-data.sh
EXPOSE 27017
VOLUME /home/ec2-user/data/db