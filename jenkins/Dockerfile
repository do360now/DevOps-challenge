FROM jenkins/jenkins:lts
WORKDIR /var/jenkins_home
RUN mkdir sonar-scanner 
RUN cd / mkdir sonar-scanner
RUN wget https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-3.3.0.1492-linux.zip
RUN unzip sonar-scanner-cli-3.3.0.1492-linux.zip
COPY ./plugins.txt /usr/share/jenkins/ref/plugins.txt
#Update the username and password
ENV JENKINS_USER admin
ENV JENKINS_PASS ThisIs@StrongP@ssword
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
RUN echo 2.0 > /usr/share/jenkins/ref/jenkins.install.UpgradeWizard.state