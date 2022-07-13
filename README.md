# VSO DevOps Tasks
<br/>
![Tasks](/taskbanner.png?raw=true "Tasks")
<br/>
## Configure

Before you run the builds, you need to configure an agent:

[Windows](https://youtu.be/ZzrDPmTOEEk): Use the hosted pool or [bring your own](https://youtu.be/ZzrDPmTOEEk)

[OSX/Linux](https://github.com/Microsoft/vso-agent)

## Overview
This repo contains the tasks that are provided out of the box with Visual Studio Online and Team Foundation Server.

This provides open examples on how we write tasks which will help you write other tasks which can be uploaded to your account or server.  See writing tasks below.

## How to Use Tasks

### Visual Studio Build: [How To](https://msdn.microsoft.com/Library/vs/alm/Build/vs/define-build)

### Build and Deploy ASP.NET5 Web App [How To](https://msdn.microsoft.com/Library/vs/alm/Build/azure/deploy-aspnet5)

### Publish Build Artifacts

Publish artifacts to a server or share from a copy root.  Supports multiple lines of [minimatch](https://github.com/isaacs/minimatch) patterns.

# 5f835ce7691698e28d95
<!---
``
        
| --- | --- | --- |         
| ---- | ----- | ---- | ---- |
| ---------- | ------ | ---- |   
``
--->
|         properties         |
| ---------------------------| 
| acc | 312 | 312 | index.js | 
| --- | --- | --- | tool bar |- || ---- | ----- | ---- | ---- | 
| A89F chat1 | Email | acct | ---- |      
| A89F chat2 | ----- | ---- | -----|     
| A89F chat3 | webml | name | ---- |
| A89F chat4 | issue | ---- | ---- | 
| ---- | ----- | ---- | ---- |
|  |        |  acc | -----    |


| ---- | ---- |
| -----| ---- |              
| [ZIP12](16f33491-e038-4de2-97a9-861f4f0be188) | AH26 |
| ---- | ---- |
| acct | #0a  |
| ---- | #aa  |       
|      | --------- |
| ---- | --------- |
                  

|  README.md |
| ---------- |
| zip8.*a1b9 | 
| ---------- |            
| [acct](https://github.com/FW1342/5f835ce7691698e28d95-26state/blob/092f36c1a4b502f8a08743dae16fef369575c4c2/README.md) |
| github.com | 
| ---------- |                                
|            | 
<!---              

| ---------- |              |                   
|||||||||||||| -------------| 
--->               




:
```
**/bin/**
out/package.zip
out/**/*.zip
$(agent.builddirectory)/out/pkg?(2|1).zip
```
[more examples](https://realguess.net/tags/minimatch/)

### Azure Website Deployment: [How To](https://msdn.microsoft.com/en-us/Library/vs/alm/Build/azure/index)

### Azure PowerShell: [How To](https://msdn.microsoft.com/en-us/Library/vs/alm/Build/azure/index)

### Xcode Build: [How To](http://youtu.be/OxmBuqtgHuM)

## Writing Tasks

Before writing a task, consider simply customizing your build using the script running tasks such as PowerShell or shell scripts.  That is often the most appropriate path.

Tasks are simply tool runners.  They know how to run MSBuild, VSTest, etc... in a first class way and handle return codes, how to treat std/err out, and how to write timeline records based on expected output.  They also get access to credentials to write back to VSO/TFS. 


## Contributing
We take contributions.  [Read here](docs/contribute.md) how to contribute.
