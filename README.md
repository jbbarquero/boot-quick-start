## Info

Simple [Spring Boot](http://projects.spring.io/spring-boot/) project to create a REST service which source fits in a tweet:

    @RestController
    public class HelloController {
        @RequestMapping("/")
        public String hello() {
            return "Hello World!";
        }
    }


## Obtaining, building and running

Download the source:

    git clone ...

Build the project

    mvn clean verify

    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time: 20.387 s
    [INFO] Finished at: 2016-08-04T09:11:26+02:00
    [INFO] Final Memory: 30M/331M
    [INFO] ------------------------------------------------------------------------

Run the application

    $ java -jar target/boot-quick-start-0.0.1-SNAPSHOT.jar

    ...
    2016-08-04 09:12:51.748  INFO 11170 --- [           main] c.m.b.demos.BootQuickStartApplication    : Started BootQuickStartApplication in 4.857 seconds (JVM running for 5.437)

Try it

    http://localhost:8080/

## Notes

    $ ls -la target/boot-quick-start-0.0.1-SNAPSHOT.jar

    -rw-rw-r-- 1 jbeneito jbeneito 14111110 ago  4 09:11 target/boot-quick-start-0.0.1-SNAPSHOT.jar
