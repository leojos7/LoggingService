## LoggingService

#### **Zero Configuration Logging**

By default the log level is at _DEBUG_ mode for the package com.learn.spring.

For getting logs at trace level we can use the below command :- 

`mvn spring-boot:run -Dspring-boot.run.arguments=--logging.level.com.learn.spring=TRACE`

#### **Logback Configuration Logging**

We have added logback-spring.xml in this version of logging.

This will create all the application logs inside LOGS folder with different colour configurations mentioned inside logback file.

#### **Log4j2 Configuration Logging**

We have to modify spring-boot-web to below dependency :-

`<dependency>
     <groupId>org.springframework.boot</groupId>
     <artifactId>spring-boot-starter-web</artifactId>
     <exclusions>
         <exclusion>
             <groupId>org.springframework.boot</groupId>
             <artifactId>spring-boot-starter-logging</artifactId>
         </exclusion>
     </exclusions>
 </dependency>
 <dependency>
     <groupId>org.springframework.boot</groupId>
     <artifactId>spring-boot-starter-log4j2</artifactId>
 </dependency>`
 
 Then create a new xml configuration for Log4j2 named log4j2-spring.xml
 
 
 
