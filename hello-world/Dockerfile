# FROM tomcat:latest
# RUN cp -R  /usr/local/tomcat/webapps.dist/*  /usr/local/tomcat/webapps
# COPY ./*.war /usr/local/tomcat/webapps


FROM tomcat:9.0-jdk11

# Remove default apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy WAR into Tomcat
COPY hello-world/webapp/target/*.war /usr/local/tomcat/webapps/webapp.war
EXPOSE 8080

CMD ["catalina.sh", "run"]

