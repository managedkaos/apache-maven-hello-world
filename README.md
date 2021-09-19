# Apache Maven 'Hello World!"
This is a small project for demonstrating the Apache Maven build management tool.

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
