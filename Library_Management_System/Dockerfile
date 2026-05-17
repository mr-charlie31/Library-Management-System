FROM tomcat:9.0-jdk11-openjdk-slim

# Remove default Tomcat apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy your local web files (HTML, JSP, WEB-INF/web.xml) into Tomcat
COPY ./WebContent /usr/local/tomcat/webapps/ROOT

EXPOSE 8080
CMD ["catalina.sh", "run"]