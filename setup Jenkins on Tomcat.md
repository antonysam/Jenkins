In default jenkins will run in standalone (jetty winstone)
but can also deploy in Tomcat server

# Links 
1. tomcat.apache.org

Note: To change the port no of Tomcat server conf/server 
      search for connector in the xml file and give the port no
      
# steps to be followed to deploy jenkins in tomcat on Windows
```
1. Download tomcat from the above link
2. Extract and place tomcat folder at any location in the machine
3. Copy/place jenkins.war inside tomcat/webapps folder 
4. Goto cmd navigate to bin folder and type startup.bat 
5. The Tomcat cmd window will run the jenkins.war file
```
