# Maven archetypes

#### Basic java project
```
mvn archetype:generate \
    -DartifactId=ProjectName \
    -DgroupId=com.example \
    -DarchetypeArtifactId=maven-archetype-quickstart \
    -DinteractiveMode=false
```

#### Tomcat
```
mvn archetype:generate \
    -DarchetypeArtifactId=maven-archetype-webapp \
    -DinteractiveMode=false \
    -DgroupId=com.example \
    -DartifactId=ProjectName
```

#### Jersey + Grizzly2 (embed http server + servlet container)
```
mvn archetype:generate \
    -DarchetypeArtifactId=jersey-quickstart-grizzly2 \
    -DarchetypeGroupId=org.glassfish.jersey.archetypes \
    -DinteractiveMode=false \
    -DgroupId=com.example \
    -DartifactId=ProjectName \
    -Dpackage=com.example.project \
    -DarchetypeVersion=2.17
```
run project with :
```
mvn exec:java
```
access to default content at : http://localhost:8080/myapp/myresource/
