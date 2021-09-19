# Apache Maven 'Hello World!"
This is a small project for demonstrating the Apache Maven build management tool.

## Generating the Code
The code for this project was created using the following script:

```
wget https://raw.githubusercontent.com/github/gitignore/master/Maven.gitignore -O .gitignore
mvn archetype:generate -DgroupId=com.learningjenkins -DartifactId=hello -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false
sleep 1
cd hello/ && mvn package
mv pom.xml src/ target/ ..
cd .. && rm -rvf hello/
```

## Building the Project with Maven
To build the project with Maven, clone the repo and run the following command inside the repo:

```
mvn package
```

## Testing the Project with Java
The project includes a [very simple test](src/test/java/com/learningjenkins/AppTest.java) that demonstrates an assertion that will always pass.

To test the actual project, a call to the package may be used with the following command:

```
java -cp target/hello-1.0-SNAPSHOT.jar com.learningjenkins.App
```
