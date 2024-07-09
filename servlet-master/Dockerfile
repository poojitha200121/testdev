# Start with a base image containing OpenJDK and Tomcat
FROM tomcat:9.0-jdk11

# Maintainer of the image
LABEL maintainer="your-email@example.com"

# Add the WAR file to the Tomcat webapps directory
COPY target/my-servlet-project.war /usr/local/tomcat/webapps/

# Expose the default Tomcat port
EXPOSE 8082

# Start Tomcat
CMD ["catalina.sh", "run"]
