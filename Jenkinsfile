pipeline {
       agent any

       stages {
           stage('Build') {
               steps {
                   git url: 'https://github.com/yourusername/java-docker-jenkins.git', branch: 'main'
                   sh 'mvn clean install'
               }
           }

           stage('Test') {
               steps {
                   sh 'java -jar target/app.jar'
               }
           }
       }
   }
