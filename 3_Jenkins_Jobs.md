# Now we will create 4 jobs on Jenkins

- githubpull
- Build & Code Review
- Unit Test
- Deploy




## 1) **githubpull** 
- install **Git** Plugin
- New Item
- Give name **githubpull**
- Freestyle Project
- ok
- advanced
- use custom workspace
```
${JENKINS_HOME}/workspace/SampleWebbApp
```
- Source Code Management
- git
```
https://github.com/RayanAhmed2000/SampleWebApp.git
```
- apply
- save

## 2) **Build & Code Review**
- install plugin **warnings next generation**
- install plugin **ant**
- new item
- buildandcodedeploy
- Freestyle Project
- ok
- advanced
- use custom workspace
```
${JENKINS_HOME}/workspace/SampleWebbApp
```
- Source Code Management
- git
```
https://github.com/RayanAhmed2000/SampleWebApp.git
```
- buid
- add build step
- invoke ant
- post build action
- add post build action
- Record compiler warnings and static analysis results
- tool
- checkstyle
- reort file pattern
```
checkstyle-result.xml
```
- apply
- save

## 3) **Unit Test**
- install plugin **warnings next generation**
- install plugin **ant**
- new item
- Unit Test
- Freestyle Project
- ok
- advanced
- use custom workspace
```
${JENKINS_HOME}/workspace/SampleWebbApp
```
- Source Code Management
- git
```
https://github.com/RayanAhmed2000/SampleWebApp.git
```
- buid
- add build step
- invoke ant
- Target
- junit
- post build action
- add post build action
- Publish JUnit test result report
```
TestCalculator_JUnitResult.xml
```
- apply
- save


## 4) **Deploy**
- install plugin **deploy to container**
- New Item
- Give name **Deploy**
- Freestyle Project
- ok
- advanced
- use custom workspace
```
${JENKINS_HOME}/workspace/SampleWebbApp
```
- Source Code Management
- git
```
https://github.com/RayanAhmed2000/SampleWebApp.git
```
- build
- add build step
- invoke ant
- target
- war
- post build action
- Deploy war/ear to a container
- WAR/EAR files
- **/*.war
- Context path
- samplewebapp
- Containers
- Add containers
- Tomcat 9.x Remote
- Credentials
- Add
- Jenkins
- Username (RayanAhmed)
- Password (admin)
- select RayanAhmed/****
- Tomcat URL
```
https://localhost:8080
```
- apply
- save


