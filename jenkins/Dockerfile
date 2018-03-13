FROM centos
MAINTAINER jack
COPY jdk1.7.0_79 /home/jdk1.7.0_79
COPY jenkins.war /home/jenkins.war
ENV JAVA_HOME=/home/jdk1.7.0_79
ENV PATH=$JAVA_HOME/bin:$PATH
ENV CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
EXPOSE 8080
WORKDIR /home
ENTRYPOINT ["java","-jar","jenkins.war"]

