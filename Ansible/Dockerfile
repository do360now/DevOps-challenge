FROM ubuntu:20.04
RUN apt update
RUN apt install software-properties-common
RUN apt-add-repository --yes --update ppa:ansible/ansible
RUN apt install ansible -y 
RUN mkdir challenge
COPY challenge-deploy.yml /challenge/challenge-deploy.yml
CMD /challenge/challenge-deploy.yml
