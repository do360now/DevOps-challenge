FROM jenkins/jenkins:lts
WORKDIR /var/jenkins_home
RUN mkdir sonar-scanner 
RUN mkdir git_repo
RUN cd sonar-scanner
RUN wget https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-3.3.0.1492-linux.zip
RUN unzip sonar-scanner-cli-3.3.0.1492-linux.zip

