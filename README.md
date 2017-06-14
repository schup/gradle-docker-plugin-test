# gradle-docker-plugin-test

# Steps    
    gradle dockerCreateNetwork
    gradle dockerRmNetwork
    
    
    $ gradle --version
    ------------------------------------------------------------
    Gradle 3.5
    ------------------------------------------------------------
    
    Build time:   2017-04-10 13:37:25 UTC
    Revision:     b762622a185d59ce0cfc9cbc6ab5dd22469e18a6
    
    Groovy:       2.4.10
    Ant:          Apache Ant(TM) version 1.9.6 compiled on June 29 2015
    JVM:          1.8.0_121 (Oracle Corporation 25.121-b13)
    OS:           Linux 4.11.3-202.fc25.x86_64 amd64


    $ docker version
    Client:
     Version:         1.12.6
     API version:     1.24
     Package version: docker-common-1.12.6-6.gitae7d637.fc25.x86_64
     Go version:      go1.7.4
     Git commit:      ae7d637/1.12.6
     Built:           Mon Jan 30 16:15:28 2017
     OS/Arch:         linux/amd64
    
    Server:
     Version:         1.12.6
     API version:     1.24
     Package version: docker-common-1.12.6-6.gitae7d637.fc25.x86_64
     Go version:      go1.7.4
     Git commit:      ae7d637/1.12.6
     Built:           Mon Jan 30 16:15:28 2017
     OS/Arch:         linux/amd64

Tested docker versions
- 17.05.0-ce on CentOS Linux release 7.3.1611 (Core)
- 1.12.6 on Fedora release 25 (Twenty Five)
   
Works with OpenJDK 1.8.0_131

## Remote
    gradle -Ddocker.host="http://docker:2375/" dockerVersion
    
## Local 
   gradle dockerVersion