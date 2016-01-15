Purpose of this project: Try to expose a REST into [Open CMS](http://www.opencms.org/en/). More specifically we try to expose an interface to an older version 8.x version. 

Usage: 

1. Download this project.
1. Setup Open CMS: Install [docker-compose](https://docs.docker.com/compose/) and call `docker-compose up` inside the downloaded project folder. 
1. After Tomcat has started go to `localhost:8888/opencms/setup` to start the installation process.
1. With Open CMS installed we can go to `spring-boot/` folder. Find opencms.properties inside and ensure the database connection settings are setup properly.
1. Call `./gradlew run` inside the `spring-boot/` folder to start the application. Word of warning. The application does not do a lot at all. Only tries to see if it can properly initalize a connection to Open CMS all the while exposing a rest interface outwards.

