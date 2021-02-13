FROM rmohr/activemq:5.15.6
COPY  mysql-connector-java-5.1.49.jar lib/
COPY activemq.xml conf/
COPY waitforit.sh .
CMD [ "./waitforit.sh", "mysql:3306", "--", "bin/activemq", "console" ]