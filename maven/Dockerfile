FROM maven:3.8.4-jdk-8 AS build
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/boxfuse-sample-java-war-hello-war-hello
RUN mvn -f /tmp/boxfuse-sample-java-war-hello-war-hello/pom.xml clean package
RUN mkdir /data
RUN cp /tmp/boxfuse-sample-java-war-hello-war-hello/target/hello-*.war /data