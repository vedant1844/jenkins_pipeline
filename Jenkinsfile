pipeline {
       agent any

       stages {
           stage('Build') {
               steps {
                   git url: 'https://github.com/vedant1844/jenkins_pipeline.git', branch: 'main'
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
