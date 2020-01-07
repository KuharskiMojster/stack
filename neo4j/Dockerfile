FROM graphfoundation/ongdb:3.5

WORKDIR /app

RUN mkdir -p /app/conf

COPY ./conf/* /app/conf/

RUN cat /app/conf/* >> /var/lib/neo4j/neo4j.conf

ENTRYPOINT ["/sbin/tini", "-g", "--", "/docker-entrypoint.sh"]

CMD ["neo4j"]
