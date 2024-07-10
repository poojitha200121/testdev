
# Use the official Tomcat base image
FROM tomcat:9.0

# Maintainer of the image (optional)
# LABEL maintainer="your-email@example.com"

# Copy the WAR file to the webapps directory of Tomcat
COPY target/my-servlet-project.war /usr/local/tomcat/webapps/

# Change Tomcat to use port 9090 instead of 8080
RUN sed -i 's/port="8080"/port="9090"/g' /usr/local/tomcat/conf/server.xml

# Expose port 9090
EXPOSE 9090

# Start Tomcat
CMD ["catalina.sh", "run"]
