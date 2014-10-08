demo-jebc
=========

Usage
-----

```
docker run -d --name storage apemberton/jenkins-storage git clone https://github.com/apemberton/demo-jebc.git .
docker run -d --name jenkins --volumes-from storage -p 80:8080 -e JENKINS_HOME=/data/var/lib/jenkins/api-team apemberton/jenkins-enterprise
```
