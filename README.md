# SCA-Cloud-School-Application
Technical assesment for SCA Cohort 2 Cloud Bootcamp application

Involves deploying an instance from the Azure Cloud Provider and running Jenkins server on it while integrating my python application via github repository.

**Link to server : http://40.114.122.41:8080/**

 **Username: admin**

 **Password: testuser12**

I have set up an instance on Azure where I will install and run Jenkins.

![azure instance](https://user-images.githubusercontent.com/42536943/126764773-9703c1ab-7a6f-451d-9fc6-8483a7d42c0f.JPG)


In the Jenkinsfile I have defined 3 stages in the pipeline which are build, Linting and deploy

![jenkinsfile](https://user-images.githubusercontent.com/42536943/126755704-60fcbe4c-e8a8-469b-85a1-7353ed62857e.JPG)


**Source(git)** - Using the git plugin I connected the github repo to Jenkins and automatically initiate a build anytime a new commit is made.

**Build/package** - In the Jenkinsfile, I created a stage called 'build' where I execute my python file.

**Deploy** - In the deploy stage one can define the steps needed to deploy their work to a server. It is the last stage and it will only run if the previous stages executed successfully.

![pipelinejenkins](https://user-images.githubusercontent.com/42536943/126755318-8cf3063e-7f0b-489c-8a84-f19f409e3220.JPG)

