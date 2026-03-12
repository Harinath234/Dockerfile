FROM amazonlinux:2023
RUN yum update -y && \ yum install -y java-21-amazon-corretto wget unzip shadow-utils procps && \ yum clean all
RUN useradd -m sonar
WORKDIR /opt
COPY sonarqube /opt/sonarqube
RUN chown -R sonar:sonar /opt/sonarqube
USER sonar
EXPOSE 9000
ENTRYPOINT ["/opt/sonarqube/bin/linux-x86-64/sonar.sh","console"]
