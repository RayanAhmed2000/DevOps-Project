# DevOps Real time Project using CI/CD Pipelines

## About Project
In this Devops Project I have created a **CI/CD Pipeline** using **Jenkins** on **Tomcat Server**. This CI/CD Pipeline will fetch code from **GitHub** and **continously check** for any updates in the code (Poll SCM), it will then **Build** and **review code** using **Ant**, then it will **test** the code and finally **deploy** the **WebApp**. All this process will be **completely automated** with **CI/CD Pipeline** starting with code fetch from **Github**


## Software installation and setup
- [Download](https://git-scm.com/downloads) and add **Git** to system enviroment variables
- [Download](https://www.oracle.com/java/technologies/downloads/) and add **JAVA** to User Variable and **Path** in system enviroment variables

- [Download](https://www.jenkins.io/download/) and install **JENKINS.WAR**

- [Download](https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.65/bin/apache-tomcat-9.0.65.exe) and install **Apache Tomcat server** 

- [Download](https://ant.apache.org/bindownload.cgi) and extract Ant 1.9.16 .zip in C: Drive

- Add **C:\apache-ant-1.9.16-bin** in user enviroment variables 
- Add **C:\apache-ant-1.9.16-bin\apache-ant-1.9.16\bin** in **Path** of System Enviroment variables

- Create a folder in C: drive named **JENKINSHOME**
- Add path of **JENKINSHOME** in system enviroment variables


## About Softwares <br>
- **Apache Tomcat Web Application Manager** - Free open source web-server widely used for hosting dynamic websites and web applications. By default it communicates on **localhost:8080**<br>
Path of webapps on local machine- <br>
**C:\Program Files\Apache Software Foundation\Tomcat 9.0\webapps**<br>
- **Ant** - Apache ANT is a Java based **build tool** from Apache Software Foundation. Apache ANT's build files are written in XML. They are open standard, portable and easy to understand.


## Steps -
- Cut Jenkins.war file and paste in C:/apache/Tomcat/Webapps
- Now Jenkisns will be visible on Tomcat -> localhost:8080
- Start the service
- Configure Jenkins
- Choose plugins to install
- Jenkins URL (in companies private IP is given but we will do it on localhost:8080)
- start


## Jobs 


