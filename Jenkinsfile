pipeline {
    agent any
    tools {

    }
    stages {
       stage ('Build') {
         steps {
         echo 'Building app...'
         script {
             'mvn build'
             }
          echo 'Building succeded!'
          }
       }
    }
}