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
    }
}