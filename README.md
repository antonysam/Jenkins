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
Will generate a key in the cmd screen

can add the maven plugin from the manage plugin tab

# Configuration

1. Select the new item name
2. Click the freestyle project 
3. Click git under the source code managemant 
4. Under build select the `Invoke top-level Maven targets`
5. Provide `clean install` in the Goals and options 
6. Post Build Actions select publish TestNG Results 
7. click on apply and save
8. select build now
9. TestNG XML report will be created and the path will be displayed in the jenkins console

# Explanation

1. While executing through jenkins, it will create a seperate workspace 

2. Get the data from the Github-pom.xml->has all the dependencies and the testNG.xml file location

3. Initially it will download all the dependencies from the maven cloud repo and execute the testcase defined the TestNG.xml file

# For adding the Java JDK in jenkins
1. Jenkins > Manage Jenkins > Manage Nodes > configure icon

2. scroll down to node properties select `Environment Variables` and define name as ` java.home` path ->provide the JDK filepath


