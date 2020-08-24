## LoggingService

#### **Zero Configuration Logging**

By default the log level is at _DEBUG_ mode for the package com.learn.spring.

For getting logs at trace level we can use the below command :- 

`mvn spring-boot:run -Dspring-boot.run.arguments=--logging.level.com.learn.spring=TRACE`

#### **Logback Configuration Logging**

We have added logback-spring.xml in this version of logging.

This will create all the application logs inside LOGS folder with different colour configurations mentioned inside logback file.


