# CiscoLive-BRKDEV2291

### Jenkins Plugins

-  [Simple theme](https://tobix.github.io/jenkins-neo2-theme/dist/neo-light.css)
-  [Docker](https://plugins.jenkins.io/docker-plugin/)
-  [Ansible](https://plugins.jenkins.io/ansible/)
-  [Build user vars](https://plugins.jenkins.io/build-user-vars-plugin/)
-  [Build Timestamp](https://plugins.jenkins.io/build-timestamp/)
-  [Notification](https://plugins.jenkins.io/notification/)
-  [AnsiColor](https://plugins.jenkins.io/ansicolor/)

### Jenkins docker container
```html
docker run -p 8080:8080 -p 50000:50000 -v /Users/saukotha/jenkins-set-up/jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```

### Expose docker desktop on port 2375
```html
docker run -d -v /var/run/docker.sock:/var/run/docker.sock -p 127.0.0.1:2375:2375 bobrik/socat TCP-LISTEN:2375,fork UNIX-CONNECT:/var/run/docker.sock
```
### Show running containers
```html
docker ps --format "table {{.Image}}\t\t{{.State}}\t\t{{ .Status }}"
```
