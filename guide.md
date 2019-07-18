# Follow this guide for running jobs on Jenkins
Xebia Jenkins URL- 192.168.7.41:8080
## Yes-genie-app - CI
Follow these steps to run CI/CD on *xebia-qa environment*

**INFO**\
CI on\
Environment-> xebia-qa\
Branch-> Xebia-QA
```
Sync job from github to gitlab is not required since we are using github for xebia-qa
```
- Step 1. Go to 192.168.7.41:8080
- Step 2. Open the folder named release-pipeline -> xebia_qa -> yes-genie-app
- Step 3. For running CI open yes-genie-app-sprint-ci
- Step 4. Click on Build with Parameters option on the left
- Step 5. Give the branch name and click Build

Check your build steps
1. Click on the build number under build history on the left
2. Click on console output
 OR
Directly click on the blue button on the left of build number 
```
Result : Image pushed with tag 1.1.0-alpha(x)
```
## Yes-genie-app - CD
**INFO**\
CD on\
Environment-> xebia-qa\
Branch-> Xebia-QA

- Step 1. Go to 192.168.7.41:8080
- Step 2. Open the folder named release-pipeline -> xebia_qa -> yes-genie-app
- Step 3. For running CD open yes-genie-app-cd-sprint-qa
- Step 4. Click on Build with Parameters option on the left
- Step 5. Give the image tag formed from CI (1.1.0-alpha(x)) and branch name then click Build

Check your build steps 
1. Click on the build number under build history on the left
2. Click on console output
 OR
Directly click on the blue button on the left of build number 
```
Version: yes-genie-app-1.1.0-alpha(x)
```

