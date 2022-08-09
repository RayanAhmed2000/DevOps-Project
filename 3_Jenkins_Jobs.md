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



## 3) **Unit Test** 
## 4) **Deploy** 

