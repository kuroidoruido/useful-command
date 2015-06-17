# Maven archetypes

#### Basic
```
mvn archetype:create
    -DgroupId=group.id.name 
	-DartifactId=ProjectName
	-Dpackagename=package.name
```
#### Tomcat
```
mvn archetype:generate 
    -DgroupId=group.id.name 
    -DartifactId=ProjectName 
    -DarchetypeArtifactId=maven-archetype-webapp 
    -DinteractiveMode=false
```
#### Jersey + Grizzly2 (embed http server + servlet container)
```
mvn archetype:generate
    -DarchetypeArtifactId=jersey-quickstart-grizzly2
    -DarchetypeGroupId=org.glassfish.jersey.archetypes
    -DinteractiveMode=false
    -DgroupId=com.example
    -DartifactId=Project
    -Dpackage=com.example.project
    -DarchetypeVersion=2.17
```
run project with :
```
mvn exec:java
```
access to default content at : http://localhost:8080/myapp/myresource/
