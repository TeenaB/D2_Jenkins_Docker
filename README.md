This repository contains a java application that is build and tested using Jenkins.
STEPS:     
  A. Install Jenkins locally and run the Jenkins server at http://localhost:8080
  B. Create a simple JAVA application and build it using MAVEN locally [This is to ensure that the application is build sucessfully]. Use commands [a] mvn clean [b] mvn clean package.
  ![image](https://github.com/user-attachments/assets/237eefc0-f77b-4c1b-a484-fd705860b41c)
  C. Create a pipeline job in Jenkins. Configure Jenkins to pull the code from SCM (Github), by giving repository URL, username and password.
  D. Add MAVEN plugins and configure JDK & MAVEN in Jenkins (Jenkins dashboard > Manage Jenkins > Tools)
  ![image](https://github.com/user-attachments/assets/3620212c-a293-4d5b-a8c7-d663b10631ec)
  ![image](https://github.com/user-attachments/assets/12cfd7f9-37e2-4105-be6c-619f5f7021a2)
  E. Write scripted pipeline instructions in **Jenkinsfile**
  
