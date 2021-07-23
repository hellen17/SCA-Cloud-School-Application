# SCA-Cloud-School-Application
Technical assesment for SCA Cohort 2 Cloud Bootcamp application

Involves deploying an instance from the Azure Cloud Provider and running jenkins server on it while integrating my python application via github repository.

In the Jenkinsfile I have defined 3 stages in the pipeline which are build, Linting and deploy

![jenkinsfile](https://user-images.githubusercontent.com/42536943/126755704-60fcbe4c-e8a8-469b-85a1-7353ed62857e.JPG)

**Source(git)** - Using the git plugin I connected the github repo to Jenkins and automatically initiate a build anytime a new commit is made.

**Build/package** - In the Jenkinsfile, I created a stage called 'build' where I execute my python file.

**Deploy** - In the deploy stage one can define the steps needed to deploy their work to a server

![pipelinejenkins](https://user-images.githubusercontent.com/42536943/126755318-8cf3063e-7f0b-489c-8a84-f19f409e3220.JPG)

