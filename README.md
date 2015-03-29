zap-maven-plugin2
------
Cloned from https://code.google.com/p/zap-maven-plugin/

ZAP Maven Plugin2 is a Maven plugin that automates dynamic security scans with the OWASP ZAP Proxy with the latest client api.

###To build
1. install ZAP clientjar in the local Maven repository with 
```sh
mvn install:install-file -Dfile=zap-api-v2-4.jar -DgroupId=org.zaproxy -DartifactId=clientapi -Dversion=2.4 -Dpackaging=jar
```

2. Run
```sh
mvn clean install 
```

###To use
2. Run 
```sh
mvn install -Ptest
```
to start ZAP and perform a scan against http://localhost:8070


### Todo's

 - Write Tests
 - Fix scanid
 - Open up more configuration options

### License


Apache License 2.0
see https://www.apache.org/licenses/LICENSE-2.0
