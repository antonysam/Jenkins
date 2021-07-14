# Jenkins
Jenkins setup

Distribution: war

# Pre-requisite
1. Java 1.8 version should be installed 
2. Download the jenkins war file from Stable(LTS)
3. link: https://www.jenkins.io/download/

# Cmd
```
java -jar <"path_of_jenkins.war_file">
```
_To configure jenkins in custom port_

# Cmd
```
java -jar <"path_of_jenkins.war_file"> --httpPort=<"port_no">
```

It will setup a webroot directory
Will get a key in the cmd screen

can add the maven plugin from the manage plugin tab

# Configuration

1. Select the new item name
2. Click the maven project 
3. Click git under the source code managemant 
4. Under build provide the pom.xml as the Root POM which will download all the artifacts
5. Provide clean install in the Goals and options 
6. Post Build Actions select publish TestNG Results 
7. click on apply and save
8. select build now
