pipeline {
        agent any

        Stages {
            Stage('checkout') {
                 Steps {
                         checkout scm
                       }}
                Stage('Build') {
                  Steps {
                         sh '/home/amrita/Documents/devops-tools/apache-maven-3.9.1/bin/mvn install'
                         }}
                Stages('Deployment'){
                  Steps {

                        sh 'cp target/Nykaa.war /home/amrita/Documents/devops-tools/apache-tomcat-9.0.73/webapps'
       }
}}}

