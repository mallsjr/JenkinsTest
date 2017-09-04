pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        sh 'echo \'Building..\''
        sh 'mvn clean'
      }
    }
    stage('TEST') {
      steps {
        sh 'echo \'Testing..\''
      }
    }
    stage('DEPLOY') {
      steps {
        sh 'echo \'Deploying..\''
      }
    }
  }
}