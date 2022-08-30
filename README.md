## The purpose of the project is to get the simplest and basic spring mvs + Tomcat configuration

1. Configure pom.xml file:
 - Important to  be added for the web app:
```
<packaging>war</packaging>

<build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-war-plugin</artifactId>
                <version>3.3.0</version>
            </plugin>
        </plugins>
</build>
```
 - Important and minimum dependencies needs to be added:
 ```
 <dependencies>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>javax.servlet-api</artifactId>
            <version>4.0.1</version>
        </dependency>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.3.12</version>
        </dependency>
 </dependencies>
 ```
 2. Create configuration classes - config package
 3. Create controllers - controller package
 4. Add Tomcat build configuration (9.0.59 currently was used)

 