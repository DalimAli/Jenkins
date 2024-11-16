# Jenkins

### start a container
docker run --name myjenkins -p 8080:8080 -p 50000:50000 -v /var/jenkins_home jenkins/jenkins:latest

## install maven using
### docker exec -it -u root DockerContainerId /bin/bash
### apt-get update
### apt-get install maven
