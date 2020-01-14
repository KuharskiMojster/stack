FROM graphfoundation/ongdb:3.5

ADD ./conf /conf

ADD ./plugins /var/lib/neo4j/plugins

ENTRYPOINT ["/sbin/tini", "-g", "--", "/docker-entrypoint.sh"]

CMD ["neo4j"]

