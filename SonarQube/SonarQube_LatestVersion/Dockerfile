FROM eclipse-temurin:21-jdk-jammy
RUN useradd -m sonar
WORKDIR /opt
COPY sonarqube /opt/sonarqube
RUN chown -R sonar:sonar /opt/sonarqube
USER sonar
EXPOSE 9000
ENTRYPOINT ["/opt/sonarqube/bin/linux-x86-64/sonar.sh","console"]
