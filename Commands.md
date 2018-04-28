##Docker With jenkins

#pull docker image from docker hub
https://hub.docker.com/r/jenkins/jenkins/

#Run the docker image with port forwarded_port
docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts

# Create a new project

1) Click on New Item of Free Style project type
2) Under General GitHub project add the project URL
    https://github.com/anubhawsinha13/maven-project-1
2) Source Code management select GIT and enter the git repository name.
    https://github.com/anubhawsinha13/maven-project-1.git
3) If public  repository then no credential required
4) Build Triggers
    GitHub hook trigger for GITScm polling
5) Go to the project to click on build now for jenkins to initiate the workspace.
6) In your git repository make changes and commit to test the web hook triggering the build project.
