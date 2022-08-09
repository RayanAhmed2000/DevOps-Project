# Website-Deployment-using-DevOps

Software Requirements
* Git
* Java 8 or 16 (Configure in System and Environement Variables)
```bash
  echo %Java_HOME%  //to verify Java Installation in cmd
```
* Tomcat server (localhost:8080/jenkins)
Add username and password while installation. You can use tomcat 8 if you find problem while working with jenkins.
* Jenkins (Generic Java Package (.war))
* Apache Ant
* git



## Installation

### Java Installation 
Goto [oracle website](https://www.oracle.com/java/technologies/downloads/) and download the latest java version. Install that jdk and configure the environment variables for both Users and System.
* Variable name: JAVA_HOME
* Variable value: C:\Program Files\Java\jdk-18

Add a new path in system variables
* Path: C:\Program Files\Java\jdk-18\bin


### Tomcat Installation 
Goto apache [tomcat website](https://tomcat.apache.org/download-10.cgi) and install the latest "32-bit/64-bit Windows Service Installer (pgp, sha512)" package. Provide the username and password during the Installation of Tomcat.

```bash
  localhost:8080
```
Now login through your credentials

### Jenkins Installation 
Goto jenkins.io [Jenkins website](https://www.jenkins.io/download/) and install the latest " (Generic Java Package (.war))" package.
Create one "JENKINSHOME" folder in C drive of your Windows. Edit the environment varibles, click on new and give name as "JENKINS_HOME" and path of that folder.
```bash
  localhost:8080
```
Now login through your credentials. Restart tge system to make changes persistent.

Open Monitor Tomcat from start menu. Start the Tomcat service. Copy the jenkins ".war" file and paste at "C:\Program Files\Apache Software Foundation\Tomcat 10.0\webapps" this location. This let the jenkins to run as the webapp in the tomcat server. Open new tab with "localhost:8080/jenkins", it will show to unlock jenkins by creating password. After entering the password click on "Select Plugins to Install". Click on None and then click on Install. Create admin user and clickk on "save and continue and finish".


### Ant Installation
Goto [Apache Ant website](https://ant.apache.org/bindownload.cgi) and download one bin.zip file. Extract that zip in the C drive. Goto ant foler and copy the path open the Environment Variable then User Varibles and cick on new.
* Variable name: ANT_HOME
* Variable value: C:\apache-ant-1.9.16

In system variable click on path add new and paste the "C:\apache-ant-1.9.16\bin" bin path.

```bash
  ant -veriosn
  echo %ANT_HOME%  // to check the 
```

Make one foler in c drive with name "gitworkspace", and clone the data from repository "https://github.com/bhupinderjnu/SampleWebApp". Run the Following command to clone.

```bash
  git clone https://github.com/bhupinderjnu/SampleWebApp
```


#### Jenkins Congiguration
Jenkins Plugins to Install
* github
* Warnings Next generation
* Ant
* Junit Realtime test reporter
* deploy to container

Jobs to create in jenkins
*  githubpull
* buildandcodereview
* unittest
* deploy