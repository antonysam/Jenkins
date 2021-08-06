# Steps to Automate deployment
1) Start Jenkins
2) Download Deployment as follows
   a) Manage Jenkins -> Manage Plugin -> search for deploy -> click on Deploy to container plugin
3) Restart your jenkins
4) Create a build job
5) Provide build action as execute windows batch cmd incase if it is Windows machine
6) Download a sample apache war file and place it in the jenkinshome/jobs/<"jobname">/sample.war
7) 
8) Click on Tomcat server with the suitable version available in your machine as a pre-requisite navigate to `tomcat location->conf->tomcat-users` 
  create a user in the XML file and run the tomcat server by `startup.bat` configure the Tomcat port in tomcat->conf->server.xml->search for connector and can change the port
9) Click on post build action click Deploy WAR/EAR to a container and provide the sample war file location and provide the tomcat version and credentials
