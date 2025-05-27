pipeline {
    agent any

    tools {
        maven "MAVEN"
        jdk "JDK"
    }

    stages {
        stage('Initialize'){
            steps{
                echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /opt/maven"
            }
        }
        stage('Build') {
            steps {
                echo 'Building now'
                bat 'mvn clean package'
                //dir("/var/lib/jenkins/workspace/New_demo/my-app/") {
                //sh 'mvn -B -DskipTests clean package'
                }
            
            }
        
       stage('Post Build') {
           steps {
               junit '*/test-results/test/*.xml'
           }
       }
    }
} 
 
