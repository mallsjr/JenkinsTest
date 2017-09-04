pipeline {
  agent any
  tools {
  	maven 'Maven 3.5.0'
  }
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