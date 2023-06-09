pipeline {
        agent any

        stages {
            stage('checkout') {
                 steps {
                         checkout scm
                       }}
                stage('Build') {
                  steps {
                         sh '/home/amrita/Documents/devops-tools/apache-maven-3.9.1/bin/mvn install'
                         }}
                stages('Deployment'){
                  Steps {

                        sh 'cp target/Nykaa.war /home/amrita/Documents/devops-tools/apache-tomcat-9.0.73/webapps'
       }
}}}

