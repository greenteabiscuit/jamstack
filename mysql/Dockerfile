FROM mysql:8.0.21
# FROM mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca

RUN echo "USE mysql;" > /docker-entrypoint-initdb.d/timezones.sql &&  mysql_tzinfo_to_sql /usr/share/zoneinfo >> /docker-entrypoint-initdb.d/timezones.sql

COPY ./my.cnf /etc/mysql/conf.d/my.cnf