# How to change configuration of Tomcat locally

## Changing port number
```
C:\Program Files\Apache Software Foundation\Tomcat 9.0\conf\server.xml
```
- Connector Port 
- edit it and save


## Granting Admin Rights to User
```
C:\Program Files\Apache Software Foundation\Tomcat 9.0\conf\tomcat-users.xml
```
``` 
<user username="admin" password="admin" roles="manager-gui"/>
```
- change it and add admin to roles

```
<user username="admin" password="admin" roles="manager-gui,admin"/>
```
