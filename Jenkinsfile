pipeline {
    agent any
    tools {
       maven 'Maven'
    }
    stages {
       stage ('Build') {
         steps {
         echo 'Building app...'
             sh 'mvn -B clean package'
          echo 'Building succeded!'
          }
       }

              stage ('Test') {
                   steps {
                        sh 'mvn test'
                     }
                      post {
                        always {
                           junit 'target/surefire-reports/*.xml'

                   }
               }
           }
            stage('Deliver') {
                       steps {
                           sh './jenkins/delivery.sh'

             }
          }
       }
    }