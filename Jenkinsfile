pipeline {
    agent any
    tools {
       maven 'Maven'
    }
    stages {
       stage ('Build') {
         steps {
         echo 'Building app...'
             sh 'mvn build'
          echo 'Building succeded!'
          }
       }
    }
}