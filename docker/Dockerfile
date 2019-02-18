FROM jboss/wildfly
 
ADD test.war /opt/jboss/wildfly/standalone/deployments/

 
RUN /opt/jboss/wildfly/bin/add-user.sh admin Admin#123 --silent
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]

