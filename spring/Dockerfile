# Download base image of jdk-25 from ghcr.io
FROM ghcr.io/graalvm/jdk-community:25i3

# Create a new deployment workspace

RUN mkdir workspace

# Copy JAR file into deployment workspace

COPY ./ecommerce-api-spring-1.0.0.jar /workspace/app.jar

# Allow host to bind port 1333

EXPOSE 1333

# Execute JAR file

ENTRYPOINT ["java","-jar","/workspace/app.jar"]


