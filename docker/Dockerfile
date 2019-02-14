FROM jboss/wildfly
COPY test.war /opt/jboss/wildfly/standalone/deployments/

RUN java -version

EXPOSE 8180 9990

FROM jboss/wildfly
RUN /opt/jboss/wildfly/bin/add-user.sh admin Admin#123 --silent
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]
