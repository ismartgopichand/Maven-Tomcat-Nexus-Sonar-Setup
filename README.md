yum install git maven java-openjdk11 tree -y

sudo yum install tomcat tomcat-webapps tomcat-admin-webapps tomcat-docs-webapp tomcat-javadoc -y

systemctl start tomcat

systemctl enable tomcat

/usr/share/tomcat/conf/tomcat-users.xml

<role rolename="manager-gui"/>
<user username="admin" password="admin" roles="manager-gui"/>

:wq!


/usr/share/tomcat
bin  conf  lib  logs  temp  webapps  work

cp target/java-tomcat-maven-example.war /usr/share/tomcat/webapps/


# jenkins-docker-project

Maven:

POM.XML   

extensible markup Lanaguage

Project object Model 

Lifecycle Phases :

Compile

Test : Target with surefire report

Package : war/jar/ear


clean : Deleteing target folder

Repositories: 3 

Remote : Other server

Local : /root/.m2/

Centeral : https://repo.maven.apache.org/maven2/org/

--------------------------------------
