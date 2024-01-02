WHAT DOES THIS WEB APPLICATION DO:
This web application is a simple exercise to become familiar with the basics of Spring Boot Applications and Jenkins CI/CD
The web application consists of 2 pages that show greetings to the user.


HOW TO USE THE WEB APPLICATION:
The web application is designed to be deployed on a tomcat server, accessible at port 8081,
and run through a Jenkins pipeline.
You can open up a Virtual Machine. Run Jenkins e.g. on Port 8080.
Create a pipeline and set it to access the Jenkinsfile of the Github project at
www.github.com/NiamhC503/TestSpring
On the same VM as Jenkins is running, access the deployed application at
localhost:8081/demo/.
Access the second greeting at localhost:8081/demo/hello.
